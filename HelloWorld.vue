<template>
  <div class="app d-flex ">
    <div class=" w-100  ">
      <!--Header-->
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
      <!-- Header logo -->
      <div class="d-flex w-100 position-relative  " style="height: 250px">
        <div id="logo" class="flex-col logo position-absolute start-50">
          <img src="https://img.upanh.tv/2022/10/03/Screenshot-2022-10-03-223840.png" alt="Screenshot-2022-10-03-223840.png">
          <a href="" title="" rel="home">
            <img src="https://www.canva.com/design/DAFN4iYtPE4/QFRAkf2syaYINFPcEMmPnw/edit?utm_content=DAFN4iYtPE4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="header-logo" alt="">
          </a>
        </div>
      </div>
      <!--img body-->
      <div class="d-flex w-100 position-relative ">
        <div class=" " style=" padding-left: 80px">
          <img id ="img" src="http://hstatic.net/152/1000115152/1000160147/slideshow_5.jpg?v=301" alt="">
        </div>
      </div>
      <!--Body1-->
      <div class=" row bg-light">
        <div class="d-flex">
          <div class=" bg-white " style="width: 700px; margin: 36px;">
            <div class="text-center p-2">
              <h4 >Thông tin người hiến máu</h4>
            </div>
            <div class=" w-100" style="height: 220px ">
              <div class="d-flex ps-2 pt-3">
                <div class="col-3"><img src="https://img.upanh.tv/2022/10/06/Screenshot-2022-10-06-001712.png" alt="Screenshot-2022-10-06-001712.png" ></div>
                <div class="col">
                  <h5>Ngọc Bích A, nhóm máu O</h5>
                  <span>Đã xác minh chất lượng nhóm máu đạt tiêu chuẩn</span>
                  <div class="py-2">
                    <button class=" rounded" @click="dataUser1 = !dataUser1" style="background-color: #ff4500">
                      <span class="text-white">Xem thông tin User1</span>
                    </button>
                  </div>
                    <div v-show="dataUser1">
                      <div>Họ và tên: Chu Thị Ngọc Bích </div>
                      <div>Nhóm máu: 0</div>
                      <div>Giới tính: Nữ </div>
                      <div>Địa Chỉ: Phường Thịnh Quang, Quận Đống Đa, Hà Nội</div>
                  </div>
                </div>
              </div>
            </div>
            <div class=" w-100" style="height: 220px ">
              <div class="d-flex ps-2 pt-3">
                <div class="col-3"><img src="https://img.upanh.tv/2022/10/06/Screenshot-2022-10-06-010703.png" alt="Screenshot-2022-10-06-010703.png"></div>
                <div class="col">
                  <h5>Ngọc Bích B, nhóm máu AB</h5>
                  <span>Đã xác minh chất lượng nhóm máu đạt tiêu chuẩn</span>
                  <div class="py-2">
                    <button class=" rounded" @click="dataUser2 = !dataUser2" style="background-color: #ff4500">
                      <span class="text-white">Xem thông tin User2</span>
                    </button>
                  </div>
                    <div v-show="dataUser2">
                      <div>Họ và tên: Chu Thị Ngọc Bích B</div>
                      <div>Nhóm máu: AB</div>
                      <div>Giới tính: Nữ </div>
                      <div>Địa Chỉ: Phường Thịnh Quang, Quận Đống Đa, Hà Nội</div>
                  </div>
                </div>
              </div>
            </div>
            <div class=" w-100" style="height: 220px ">
              <div class="d-flex ps-2 pt-3">
                <div class="col-3"><img src="https://img.upanh.tv/2022/10/06/Screenshot-2022-10-06-011926.png" alt="Screenshot-2022-10-06-011926.png"></div>
                <div class="col">
                  <h5>Ngọc Bích C, nhóm máu A</h5>
                  <span>Đã xác minh chất lượng nhóm máu đạt tiêu chuẩn</span>
                  <div class="py-2">
                    <button class=" rounded" @click="dataUser3 = !dataUser3" style="background-color: #ff4500">
                      <span class="text-white">Xem thông tin User2</span>
                    </button>
                  </div>
                    <div v-show="dataUser3">
                      <div>Họ và tên: Chu Thị Ngọc Bích C</div>
                      <div>Nhóm máu: A</div>
                      <div>Giới tính: Nữ </div>
                      <div>Địa Chỉ: Phường Thịnh Quang, Quận Đống Đa, Hà Nội</div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class=" bg-white " style="width: 700px; margin: 36px;">
            <div class="text-center p-2">
              <h4 >Thông tin người nhận máu máu</h4>
            </div>
            <div class=" w-100" style="height: 220px ">
              <div class="d-flex ps-2 pt-3">
                <div class="col-3"><img src="https://img.upanh.tv/2022/10/06/Screenshot-2022-10-06-013932.png" alt="Screenshot-2022-10-06-013932.png" ></div>
                <div class="col">
                  <h5>Thanh Tùng, nhóm máu B</h5>
                  <div class="py-2">
                    <button class=" rounded" @click="dataUser4 = !dataUser4" style="background-color: #ff4500">
                      <span class="text-white">Xem thông tin Bệnh Nhân</span>
                    </button>
                  </div>
                    <div v-show="dataUser4">
                      <div>Họ và tên: Nguyễn Thanh Tùng</div>
                      <div>Nhóm máu: B</div>
                      <div>Giới tính: Nam </div>
                      <div>Địa Chỉ: Phường Ngã Tư Sở, Quận Đống Đa, Hà Nội</div>
                  </div>
                </div>
              </div>
            </div>
            <div class=" w-100" style="height: 220px ">
              <div class="d-flex ps-2 pt-3">
                <div class="col-3"><img src="https://img.upanh.tv/2022/10/06/Screenshot-2022-10-06-014651.png" alt="Screenshot-2022-10-06-014651.png"></div>
                <div class="col">
                  <h5>Sơn Tùng, nhóm máu A</h5>
                  <div class="py-2">
                    <button class=" rounded" @click="dataUser5 = !dataUser5" style="background-color: #ff4500">
                      <span class="text-white">Xem thông tin Bệnh nhân</span>
                    </button>
                  </div>
                    <div v-show="dataUser5">
                      <div>Họ và tên: Nguyễn Thanh Sơn Tùng</div>
                      <div>Nhóm máu: A</div>
                      <div>Giới tính: Nam</div>
                      <div>Địa Chỉ: Phường Thịnh Liệt, Quận Đống Đa, Hà Nội</div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!--Body2-->
      <div class=" w-100 bg-light justify-content-between px-5 pb-5">
        <div class="row d-flex p-5" >
          <div class=" bg-white" style="height: 400px">
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
        </div>
        
        </div>
      <!--Body3-->
      <div class=" d-flex w-100 bg-white" style="height: 600px">
        <div style="width: 700px">
          <div class=" p-4">
          <h4>Thông tin các ca hiến máu</h4>
          </div>
          <div style="height: 200px">
          <div style="width: 600px;">
            <button class="" @click="dataUserBN1 = !dataUserBN1" style="background-color: white; width: 250px; border: white;">
              <h6 class="">Xem thông tin ca hiến máu S1</h6>
            </button>
          </div>
          <div v-show="dataUserBN1">
            <div>
              <div>Người hiến máu: Chu Thị Ngọc Bích B</div>
              <div>Người nhận Máu: Nguyễn Thanh Sơn Tùng </div>
              <div>Nhóm máu: AB</div>
              <div>Thời gian thực hiện truyền máu: 11 giờ 11 phút ngày 11 tháng 10 năm 2022</div>
              <div>Nơi thực hiện truyền máu: Bệnh viện Bạch Mai</div>
            </div>
          </div>
          </div>
          <div style="width: 500px">
            <button class="" @click="dataUserBN2 = !dataUserBN2" style="background-color: white; width: 250px; border: white;">
              <h6 class="">Xem thông tin ca hiến máu S2</h6>
            </button>
          </div>
          <div v-show="dataUserBN2">
            <div>
              <div>Người hiến máu: Chu Thị Ngọc Bích </div>
              <div>Người nhận Máu: Nguyễn Thanh Tùng </div>
              <div>Nhóm máu: O</div>
              <div>Thời gian thực hiện truyền máu: 18 giờ 33 phút ngày 11 tháng 10 năm 2022</div>
              <div>Nơi thực hiện truyền máu: Bệnh viện Bạch Mai</div>
            </div>
          </div>
          </div>
      

        <div class=" d-flex bg-white p-5 " style="width: 700px" >
          <div class="text-center">
            <h4>Quỹ ủng hộ</h4>
          </div>
          <div>
            <img src="https://store.cubemars.com/erweima_png.php?id=1030" alt="">
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
                       <p style="text-align: center;"><img class="alignnone  wp-image-774" src="https://img.upanh.tv/2022/10/03/Screenshot-2022-10-03-223840.png" alt="Screenshot-2022-10-03-223840.png"  ></p>
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
    const dataUserBN2 = ref()
    const dataUserBN1 = ref()
    const xemData = ref()
    const dataUser1 = ref()
    const dataUser2 = ref()
    const dataUser3 = ref()
    const dataUser4 = ref()
    const dataUser5 = ref()
      return{
        dataUserBN1,
        dataUserBN2,
        dataUser1,
        dataUser2,
        dataUser3,
        dataUser4,
        dataUser5,
        xemData,

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
