<template>
  <div class="about">
    <section>
      <div class="container-fluid background">
        <div class="container">
          <div class="row">
            <div class="col-md-3"></div>
            <div class="col-md-6">
              <h3 class="text-center slide_text">About Us</h3>
            </div>
            <div class="col-md-3"></div>
          </div>
        </div>
      </div>
    </section>
    <section class="ecom_about_list">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="ecom_about_inner">
              <div class="row align-items-center justify-content-between">
                <div class="col-lg-6 col-sm-6">
                  <div class="ecom_about_img">
                    <img src="@/assets/image.jpg" class="img-fluid" alt="">
                    <img src="@/assets/about_overlay.png" class="ecom_about_overlay img-fluid" alt="">
                  </div>
                </div>
                <div class="col-lg-5 col-sm-6">
                  <div class="ecom_about_content">
                    <h2>Our Mission</h2>
                    <p>Praesent posuere nec nisl quis hendrerit. Duis sit amet rutrum lorem. Ut maximus orci in metus blandit, et placerat dolor congue. Proin tempor ligula nec dolor facilisis mattis. Suspendisse potenti. Suspendisse efficitur turpis quis risus molestie cursus.</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="ecom_about_inner">
              <div class="row align-items-center justify-content-between">
                <div class="col-lg-6 col-sm-6">
                  <div class="ecom_about_img">
                    <img src="@/assets/image.jpg" class="img-fluid" alt="">
                    <img src="@/assets/about_overlay.png" class="ecom_about_overlay img-fluid" alt="">
                  </div>
                </div>
                <div class="col-lg-5 col-sm-6">
                  <div class="ecom_about_content">
                    <h2>Our Mission</h2>
                    <p>Praesent posuere nec nisl quis hendrerit. Duis sit amet rutrum lorem. Ut maximus orci in metus blandit, et placerat dolor congue. Proin tempor ligula nec dolor facilisis mattis. Suspendisse potenti. Suspendisse efficitur turpis quis risus molestie cursus.</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

    </section>
  </div>
</template>
<script>
  export default{
    name: "about",
  }
</script>
<style lang="css" scoped>
.background
{
	background-image: linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.9)),url("../assets/about_image.jpg");
  background-position: center;
  background-size: cover;
  padding: 180px 0px;
}
.slide_text{
  font-size: 81px;
  color: #fff;
}
.ecom_about_list {
  padding: 90px 0 0;
}
@media (max-width: 991px) {
  .ecom_about_list {
    padding: 90px 0 0;
  }
}
@media only screen and (min-width: 992px) and (max-width: 1200px) {
  .ecom_about_list {
    padding: 90px 0 90px;
  }
}
.ecom_about_list .ecom_about_img {
  position: relative;
  margin: 35px 0 0 35px;
}
@media (max-width: 991px) {
  .ecom_about_list .ecom_about_img {
    max-width: 204px;
  }
}
.ecom_about_list .ecom_about_img .ecom_about_overlay {
  position: absolute;
  left: -35px;
  top: -35px;
  z-index: -1;
}
.ecom_about_list .ecom_about_content h2 {
  font-size: 40px;
  line-height: 1.5;
  font-weight: 500;
  margin: 10px 0 50px;
}
@media (max-width: 991px) {
  .ecom_about_list .ecom_about_content h2 {
    font-size: 25px;
    margin: 10px 0 30px;
  }
}
@media only screen and (min-width: 992px) and (max-width: 1200px) {
  .ecom_about_list .ecom_about_content h2 {
    font-size: 30px;
    margin: 10px 0 30px;
  }
}
@media (max-width: 991px) {
  .ecom_about_list .ecom_about_content {
    margin-top: 80px;
  }
}
.ecom_about_list .ecom_about_inner {
  margin-bottom: 100px;
}
@media (max-width: 991px) {
  .ecom_about_list .ecom_about_inner {
    margin-bottom: 60px;
  }
}
.ecom_about_list .ecom_about_inner:nth-child(2n-2) .row {
  flex-direction: row-reverse;
  margin-top: 140px;
}
@media (max-width: 991px) {
  .ecom_about_list .ecom_about_inner:nth-child(2n-2) .row {
    margin-bottom: 70px;
    margin-top: 100px;
  }
}
@media (max-width: 991px) {
  .ecom_about_list .ecom_about_inner:nth-child(2n-2) .row .ecom_about_content {
    margin-top: 40px;
  }
}
.ecom_about_list .ecom_about_inner:nth-child(2n-2) .row .ecom_about_img {
  position: relative;
  margin: 0 35px 35px 0;
}
.ecom_about_list .ecom_about_inner:nth-child(2n-2) .row .ecom_about_img .ecom_about_overlay {
  position: absolute;
  left: auto;
  right: -35px;
  top: -35px;
  z-index: -1;
}
</style>
