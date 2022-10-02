<template>
  <div class="app d-flex ">
    <div class=" w-100  ">
      <div class="d-flex w-100 bg-secondary justify-content-between ps-4 " style="height: 54px">
        <div class="d-flex col-6 p-3">
          <span class="text-white text-align-center">Hiến máu cứu người - Một nghĩ cử cao đẹp. Hãy cùng giọt máu Việt cứu sống con người Việt Nam</span>
          <i class=" fa-brands fa-facebook"></i>
          <font-awesome-icon icon="fa-brands fa-facebook" />
          <i class="fab fa-facebook-square"></i>
        </div>
        <div class=" d-flex pe-4">
	        <a rel=" " href="" target="_blank" class="btn btn-primary text-align-center my-2 border" style="border-radius:6px; background-color:#ff4500; cursor: pointer; font-weight: bolder">
            <span>Đăng nhập</span>
          </a>
	      </div>
          
        
      </div>
      <div class="d-flex w-100 position-relative  " style="height: 120px">
          <div id="logo" class="flex-col logo position-absolute start-50">
            <!-- Header logo -->
            <a href="" title="" rel="home">
              <img src="https://www.canva.com/design/DAFN4iYtPE4/QFRAkf2syaYINFPcEMmPnw/edit?utm_content=DAFN4iYtPE4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="header-logo" alt="">
            </a>
          </div>
      </div>
      <div class="d-flex w-100 position-relative ">
        <div class=" " style=" padding-left: 80px">
          <img src="http://hstatic.net/152/1000115152/1000160147/slideshow_5.jpg?v=301" alt="">
        </div>
      </div>
      <div class=" row bg-light">
        <div class="d-flex">
          <div class=" bg-white " style="width: 700px; margin: 36px;">
            <div class="text-center p-2">
              <h4 >Thông tin người hiến máu</h4>
            </div>
            <div class="d-flex">
              <form class="w-100">
                <div class="w-80 px-5 " >
                  <div class="d-flex justify-content-between m-4 w-70 " >
                    <lable for=" inputFirstname" class="col-3 d-block  " >
                      <p>Tên:</p>
                     </lable>
                     <input type="inputFirstname " class="col form-control " v-model="firstName" id="inputFirstname" placeholder="name@example.com" >
                    </div>
                  <div class="d-flex justify-content-between m-4 w-70 " >
                    <label for="inputLastname" class="col-3 d-block " >
                      <p>Họ:</p>
                    </label>
                    <input type="inputLastname" class="col form-control" v-model="lastName" id="inputLastname" placeholder="name@example.com">
                  </div>
                  <div class="d-flex justify-content-between m-4 w-70 ">
                    <label for="inputAddress" class="col-3 d-block ">Address:</label>
                    <input type="inputAddress" class="col form-control" v-model="Address" id="inputAddress" placeholder="name@example.com">
                  </div>
                  <div class="d-flex justify-content-between m-4 w-70 ">
                    <label for="inputHeathl" class="col-3 d-block ">Tình trạng sức khỏe:</label>
                    <input type="inputHeathl" class="col form-control" v-model="Heathl" id="inputHeathl" placeholder="name@example.com">
                  </div>
                  <div class="d-flex justify-content-between m-4 w-70 ">
                    <p class="col-3 d-block ">Giới Tính:</p>
                  <div class="d-flex col ">
                  <input type="radio" id="male" value="Male" v-model="picked" name="radio" />
                    <label for="male">Nam</label>
                    <input type="radio" id="female" value="Female" v-model="picked" name="radio"/>
                    <label for="female">Nữ</label>
                  </div>
                </div>
                <div class="d-flex justify-content-between m-4 w-70 ">
                  <div class="col-3 d-block">
                    <p>Nhóm máu:</p>
                   </div>
                  <select class="form-select d-flex col" aria-label="Default select example" placeholder="Choix de la filiale" v-model="text">
                    <option selected>Nhóm máu A</option>
                    <option selected>Nhóm máu B</option>
                    <option selected>Nhóm máu AB</option>
                    <option selected> Nhóm máu O</option>
                  </select>
                </div>
                 <div class="btn" @click="showData = !showData" style="background-color: #ff8200">
                   <span class="text-white">Show data</span>
                  </div>
                 <div class="rounded border mt-4 " v-show="showData">
                 <div class="d-flex border-bottom">
                 <div class="col-3 border-end">
                  <span>Tên</span>
                 </div>
                 <div>
                 {{ firstName }}
                </div>
                </div>
                <div class="d-flex border-bottom">
                <div class="col-3 border-end">
                  <span>Họ</span>
                </div>
                <div>{{ lastName }}</div>
                </div>
                <div class="d-flex border-bottom ">
                <div class="col-3 border-end">
                 <span>Địa chỉ </span>
                </div>
                <div>{{ Address }}</div>
                </div>
                <div class="d-flex border-bottom ">
                <div class="col-3 border-end">
                 <span>Tình trạng sức khỏe </span>
                </div>
                <div>{{ Heathl }}</div>
                </div>
                <div class="d-flex border-bottom">
                <div class="col-3 border-end">
                 <span>Giới Tính</span>
                 </div>
                 <div>{{ picked }}</div>
                </div>
                <div class="d-flex border-bottom">
                <div class="col-3 border-end">
                 <span>Nhóm máu</span>
                </div>
                <div>{{ text }}</div>
                </div>
              </div>
              </div>
              </form>
            </div>
          </div>
          <div class=" bg-white " style="width: 700px; margin: 36px;">
            <div class="text-center p-2">
              <h4 >Thông tin người nhận máu máu</h4>
            </div>
            <div class="d-flex">
              <form class="w-100">
                <div class="w-80 px-5 " >
                  <div class="d-flex justify-content-between m-4 w-70 " >
                    <lable for=" inputFirstname1" class="col-3 d-block  " >
                      <p>Tên:</p>
                     </lable>
                     <input type="inputFirstname1 " class="col form-control " v-model="firstName1" id="inputFirstname1" placeholder="name@example.com" >
                    </div>
                  <div class="d-flex justify-content-between m-4 w-70 " >
                    <label for="inputLastname1" class="col-3 d-block " >
                      <p>Họ:</p>
                    </label>
                    <input type="inputLastname1" class="col form-control" v-model="lastName1" id="inputLastname1" placeholder="name@example.com">
                  </div>
                  <div class="d-flex justify-content-between m-4 w-70 ">
                    <label for="inputAddress1" class="col-3 d-block ">Address:</label>
                    <input type="inputAddress1" class="col form-control" v-model="Address1" id="inputAddress1" placeholder="name@example.com">
                  </div>
                  <div class="d-flex justify-content-between m-4 w-70 ">
                    <label for="inputHeathl1" class="col-3 d-block ">Tình trạng sức khỏe:</label>
                    <input type="inputHeathl1" class="col form-control" v-model="Heathl1" id="inputHeathl1" placeholder="name@example.com">
                  </div>
                  <div class="d-flex justify-content-between m-4 w-70 ">
                    <p class="col-3 d-block ">Giới Tính:</p>
                  <div class="d-flex col ">
                  <input type="radio" id="male" value="Male" v-model="picked1" name="radio" />
                    <label for="male">Nam</label>
                    <input type="radio" id="female" value="Female" v-model="picked1" name="radio"/>
                    <label for="female">Nữ</label>
                  </div>
                </div>
                <div class="d-flex justify-content-between m-4 w-70 ">
                  <div class="col-3 d-block">
                    <p>Nhóm máu:</p>
                   </div>
                  <select class="form-select d-flex col" aria-label="Default select example" placeholder="Choix de la filiale" v-model="text1">
                    <option selected>Nhóm máu A</option>
                    <option selected>Nhóm máu B</option>
                    <option selected>Nhóm máu AB</option>
                    <option selected> Nhóm máu O</option>
                  </select>
                </div>
                 <div class="btn" @click="showData1 = !showData1" style="background-color: #ff8200">
                   <span class="text-white">Show data</span>
                  </div>
                 <div class="rounded border mt-4 " v-show="showData1">
                 <div class="d-flex border-bottom">
                 <div class="col-3 border-end">
                  <span>Tên</span>
                 </div>
                 <div>
                 {{ firstName1 }}
                </div>
                </div>
                <div class="d-flex border-bottom">
                <div class="col-3 border-end">
                  <span>Họ</span>
                </div>
                <div>{{ lastName1 }}</div>
                </div>
                <div class="d-flex border-bottom ">
                <div class="col-3 border-end">
                 <span>Địa chỉ </span>
                </div>
                <div>{{ Address1 }}</div>
                </div>
                <div class="d-flex border-bottom ">
                <div class="col-3 border-end">
                 <span>Tình trạng sức khỏe </span>
                </div>
                <div>{{ Heathl1 }}</div>
                </div>
                <div class="d-flex border-bottom">
                <div class="col-3 border-end">
                 <span>Giới Tính</span>
                 </div>
                 <div>{{ picked1 }}</div>
                </div>
                <div class="d-flex border-bottom">
                <div class="col-3 border-end">
                 <span>Nhóm máu</span>
                </div>
                <div>{{ text1 }}</div>
                </div>
              </div>
              </div>
              </form>
            </div>
          </div>
        </div>
      </div>
      <div class=" w-100 bg-light justify-content-between">
        <div class="row d-flex p-5" >
          <div class=" bg-white" style="width: 1000px ">
          <div class="text-center col-inner " style="padding:0px 0px 0px 7px;">
            <div class="pt-2">
              <h5>DANH SÁCH ĐỊA ĐIỂM TRUYỀN MÁU </h5>
            </div>
          </div>
          <div class="position-relative">
            <div class="btn position-absolute top-50 start-50" @click="xemData = !xemData" style="background-color: #ff4500">
              <span class="text-white">Xem</span>
            </div>
          </div>
          <div class="pt-5">
            <div class="rounded border mt-4 " v-show="xemData">
            <div class="d-flex border-bottom">
              <div class="col-4 border-end text-center">
                <span>Miền Bắc</span>
              </div>
              <div class="col-4 border-end text-center">
                <span>Miền Trung</span>
              </div>
              <div class="col-4 text-center">
                <span>Miền Nam</span>
              </div>
              <div>
             
            </div>
          </div>
          <div class="d-flex border-bottom">
          <div class="col-4 border-end">
            <span>Viện Huyết học – Truyền máu Trung ương (Phố Phạm Văn Bạch, Cầu Giấy, Hà Nội)</span>
          </div>
          <div class="col-4 border-end">
            <span>Khoa Huyết học -Truyền máu, Bệnh viện Đà Nẵng, 103 Quang Trung (Đà Nẵng)</span>
          </div>
          <div>
            <span>Bệnh viện Truyền máu – Huyết học (118 Hồng Bàng, quận 5)</span>
          </div>
          </div>
          <div class="d-flex border-bottom ">
          <div class="col-4 border-end">
            <span>Điểm hiến máu cố định Quận Hoàn Kiếm (26 Lương Ngọc Quyến, Hà Nội)</span>
          </div>
          <div class="col-4 border-end">
            <span> Khoa Huyết học Truyền máu, Lầu 1, Bệnh viện đa khoa tỉnh Quảng Ngãi (đường Lê Hữu Trác – TP Quảng Ngãi)</span>
          </div>
          <div>
            <span>Trung tâm Hiến máu nhân đạo (106 Thiên Phước, quận Tân Bình)</span>
          </div>
          </div>
          <div class="d-flex border-bottom">
          <div class="col-4 border-end">
            <span> Điểm hiến máu cố định quận Thanh Xuân (132 Quan Nhân, Hà Nội)</span>
          </div>
          <div class="col-4 border-end">
            <span>Trung tâm Huyết học – Truyền máu, tầng 4, Bệnh viện đa khoa tỉnh Bình Định, số 106 Nguyễn Huệ, thành phố Quy Nhơn</span>
          </div>
          <div>
            <span>Bệnh viện Chợ Rẫy (tầng 1, Trung tâm Truyền máu, 201 B Nguyễn Chí Thanh, phường 12, quận 5, TPHCM)</span>
          </div>
          </div>
          <div class="d-flex border-bottom">
          <div class="col-4 border-end">
            <span>Điểm hiến máu cố định quận Đống Đa (số 10, ngõ 122 đường Láng, Hà Nội)</span>
          </div>
          <div class="col-4 border-end">
            <span></span>
          </div>
          <div>
            <span></span>
          </div>
          </div>
          <div class="d-flex ">
          <div class="col-4 border-end">
            <span>Điểm hiến máu cố định quận Ba Đình (78 Nguyễn Trường Tộ, Hà Nội)</span>
          </div>
          <div class="col-4 border-end">
            <span></span>
          </div>
          <div>
            <span></span>
          </div>
          </div>
        </div>
          </div>
        </div>
        <div class=" bg-white ms-4" style="max-width: 420px">
          <div>
            <span>Mã QR </span>
          </div>
            <div>
            <img src="https://anhong.com.vn/wp-content/uploads/2020/09/ma-qrcode-https-baohodoanhnghiep-com.png" alt="anhqr" class="">
            </div>
        </div>
      </div>
        </div>
      <footer id="footer" class="footer-wrapper">
        <section class="section" id="section_351516950">
          <div class="bg section-bg fill bg-fill bg-loaded">
          </div><!-- .section-bg -->
          <div class="section-content relative">
            <div class="row row-collapse" style="max-width:1200px" id="row-1362028200">
              <div class="col ">
                <div class="col-inner" style="padding:0px 3px 0px 11px;">
                  <div class="row" id="row-1453526420">
                    <div class="col medium-3 ">
                      <div class="col-inner">
                       <p style="text-align: center;"><img class="alignnone  wp-image-774" src="https://hienmautinhnguyen.org/wp-content/uploads/2021/10/LOGO-DOC-1-253x300.png" alt="cộng đồng hiến máu việt nam" width="136" height="161"></p>
                      </div>
                     </div>
                    <div class="col medium-9 "><div class="col-inner">
                    <div class="row row-collapse" id="row-693815721">
                    <div class="col small-12 large-12"><div class="col-inner">
                    <h2><span style="color: #ed1c24;"><strong>  GIỌT MÁU VIỆT</strong></span></h2>
                  </div>
                </div>
              </div>
            <div class="gap-element clearfix" style="display:block; height:auto; padding-top:5px"></div>
            <div class="d-flex" id="row-308356946">
            <div class="col"><div class="col-inner">
            <div class="icon-box featured-box icon-box-left text-left is-small">
            <div class="icon-box-img" style="width: 20px">
            <div class="icon">
            <div class="icon-inner">
              <img width="40px" height="40px" src="https://hienmautinhnguyen.org/wp-content/uploads/2021/08/amtp_mobile-app_-decal-dan-kinh_1100wx400h-02-300x300.png" class="attachment-medium size-medium" alt="" loading="lazy" srcset="https://hienmautinhnguyen.org/wp-content/uploads/2021/08/amtp_mobile-app_-decal-dan-kinh_1100wx400h-02-300x300.png 300w, https://hienmautinhnguyen.org/wp-content/uploads/2021/08/amtp_mobile-app_-decal-dan-kinh_1100wx400h-02-1024x1024.png 1024w, https://hienmautinhnguyen.org/wp-content/uploads/2021/08/amtp_mobile-app_-decal-dan-kinh_1100wx400h-02-150x150.png 150w, https://hienmautinhnguyen.org/wp-content/uploads/2021/08/amtp_mobile-app_-decal-dan-kinh_1100wx400h-02-768x767.png 768w, https://hienmautinhnguyen.org/wp-content/uploads/2021/08/amtp_mobile-app_-decal-dan-kinh_1100wx400h-02.png 1043w" sizes="(max-width: 300px) 100vw, 300px">					</div>
            </div>
            </div>
            <div class="icon-box-text last-reset">
              <p>Địa chỉ:&nbsp; Số 75 Tây Sơn, Đống Đa, TP Hà Nội <i class="fa-brands fa-facebook"></i><br>Email: giotmauviet@gmail.com</p>
            </div>
            </div><!-- .icon-box -->
            </div></div>
            </div>
            </div></div>
            </div>
            <p style="text-align: center; padding-left: 240px;">Trang thông tin Giọt máu Việt</p>
          </div></div>
          </div>
            <p style="text-align: center;"><span style="font-size: 80%;">Thiết kế website bởi: Julyy07</span></p>
          </div><!-- .section-content -->
        </section>
<!-- FOOTER 1 -->
<!-- FOOTER 2 -->
      <div class="absolute-footer light medium-text-center text-center">
      <div class="container clearfix">
      <div class="footer-primary pull-left">
        <div class="copyright-footer">
          </div>
      </div><!-- .left -->
      </div><!-- .container -->
      </div><!-- .absolute-footer -->
        <a href="#top" class="back-to-top button icon invert plain fixed bottom z-1 is-outline hide-for-medium circle active" id="top-link"><i class="icon-angle-up"></i></a>
    </footer>
    </div>
  </div>
  
</template>
<script>
  import { ref} from 'vue'
export default {
  setup (){
      const xemData = ref()
      const showData = ref()
      const showData1 = ref()
      const province = ref()
      const firstName = ref()
      const firstName1 = ref()
      const lastName=  ref()
      const lastName1=  ref()
      const text = ref()
      const text1 = ref()
      const Address = ref()
      const Address1 = ref()
      const picked = ref()
      const picked1 = ref()
      const Heathl =ref()
      const Heathl1 =ref()
      return{
        province,
        text,
        firstName, 
        lastName,
        Address, 
        picked, 
        showData,
        showData1,
        xemData,
        Heathl,
        firstName1,
        lastName1,
        Address1, 
        picked1,
        text1,
        Heathl1,

      }
    }
 }
</script>

<style>
  #section_351516950 {
padding-top: 30px;
padding-bottom: 30px;
background-color: rgb(229, 229, 229);
}
</style>
