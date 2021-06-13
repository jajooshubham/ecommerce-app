<template>
  <div class="home">
    <section class="background mt-5 pt-3">
      <div class="container-fluid p-0 m-0">
        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
          <ol class="carousel-indicators">
            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
          </ol>
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img class="d-block w-100" src="@/assets/about_image.jpg" alt="First slide">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="@/assets/about_image.jpg" alt="Second slide">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="@/assets/about_image.jpg" alt="Third slide">
            </div>
          </div>
          <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
      </div>
    </section>


    <section class="ecom_product">
      <div class="container-fluid my-5"
      v-for = "category in categories"
      :key = "category.name"
      >
      <div class="text-left">
        <h4 class="ecom_h4">{{ category.name }}</h4>
        <p class="ecom_p"><a href="#">View All</a></p>
      </div>
      <div class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-slide"
          v-for = "product in category.products"
          :key = "product.id"
          >
          <div class="container page-wrapper">
            <div class="page-inner">
              <div class="row">
                <div class="el-wrapper">
                  <div class="box-up">
                    <img class="img" src="http://code.slicecrowd.com/labs/4/images/t-shirt.png" alt="">
                    <div class="img-info">
                      <div class="info-inner">
                        <span class="p-name">{{ product.name }}</span>
                      </div>
                      <div class="a-size">
                        <div class="btn btn-sm btn-info">
                          <i class="fa fa-heart"></i>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="box-down">
                    <div class="h-bg">
                      <div class="h-bg-inner"></div>
                    </div>
                    <a class="cart" href="#">
                      <span class="price">$120</span>
                      <span class="add-to-cart">
                        <span class="txt">Add in cart</span>
                      </span>
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="ecom_offer">
  <div class="container-fluid my-5">
    <div class="text-left">
      <h4 class="ecom_h4">Offers</h4>
      <p class="ecom_p"><a href="#">View All</a></p>
    </div>

    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide"
        v-for="offer in offers"
        :key="offer.id"
        >
          <div class="wrapper">
            <div class="product-img">
              <img src="@/assets/image.jpg" height="420" width="327">
            </div>
            <div class="product-info">
              <div class="product-text">
                <h1>{{ offer.name }}</h1>
                <p>{{ offer.description }}</p>
              </div>
              <div class="product-price-btn">
                <button type="button">See Details</button>
                <button type="button">Buy Products</button>
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
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import product from "@/product.js"
import offer from "@/offer.js"
export default {

  name: 'Home',
  components: {},
  data() {
    return {
      categories : product.categories,
      offers : offer.offers
    }
  }
}
</script>
<style media="screen" scoped>
.background img {
  object-fit: cover;
  height: calc(100vh - 64px);
}
@media (max-width: 767px) {
  .background img {
    height: auto;
  }
}
.ecom_content{
  color: #fff;
}
.ecom_product{
  font-family: 'Roboto', sans-serif;
}
.ecom_product .ecom_h4{
  font-size: 36px;
  font-weight: 700;
  font-family: 'Raleway', sans-serif;
  margin-bottom: 20px;
  display: inline-block;
}
@media (max-width: 767px) {
  .ecom_product .ecom_h4{
    font-size: 25px;
  }
}
.ecom_product .ecom_p{
  font-size: 18px;
  float: right;
  font-family: 'Raleway', sans-serif;
  margin-bottom: 20px;
}

/*product card*/

.ecom_product .swiper-slide{
	width: 320px !important;
}
.d-flex {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}

.align-center {
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.flex-centerY-centerX {
  justify-content: center;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.page-wrapper {
  height: 100%;
  display: table;
}

.page-wrapper .page-inner {
  display: table-cell;
  vertical-align: middle;
}

.el-wrapper {
  width: 290px;
  padding: 15px;
  background-color: #fff;
}

@media (max-width: 991px) {
  .el-wrapper {
    width: 345px;
  }
}

@media (max-width: 767px) {
  .el-wrapper {
    width: 270px;
    margin: 30px auto;
  }
}

.el-wrapper:hover .h-bg {
  left: 0px;
}

.el-wrapper:hover .price {
  left: 20px;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  -o-transform: translateY(-50%);
  transform: translateY(-50%);
  color: #818181;
}

.el-wrapper:hover .add-to-cart {
  left: 50%;
}

.el-wrapper:hover .img {
  webkit-filter: blur(7px);
  -o-filter: blur(7px);
  -ms-filter: blur(7px);
  filter: blur(7px);
  filter: progid:DXImageTransform.Microsoft.Blur(pixelradius='7', shadowopacity='0.0');
  opacity: 0.4;
}

.el-wrapper:hover .info-inner {
  bottom: 155px;
}

.el-wrapper:hover .a-size {
  -webkit-transition-delay: 300ms;
  -o-transition-delay: 300ms;
  transition-delay: 300ms;
  bottom: 50px;
  opacity: 1;
}

.el-wrapper .box-down {
  width: 100%;
  height: 60px;
  position: relative;
  overflow: hidden;
}

.el-wrapper .box-up {
  width: 100%;
  height: 300px;
  position: relative;
  overflow: hidden;
  text-align: center;
}

.el-wrapper .img {
  padding: 20px 0;
  -webkit-transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  -moz-transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  -o-transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -moz-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -o-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  width: 100%;
}

.h-bg {
  -webkit-transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  -moz-transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  -o-transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  transition: all 800ms cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -moz-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -o-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  width: 660px;
  height: 100%;
  background-color: #3f96cd;
  position: absolute;
  left: -659px;
}

.h-bg .h-bg-inner {
  width: 50%;
  height: 100%;
  background-color: #464646;
}

.info-inner {
  -webkit-transition: all 400ms cubic-bezier(0, 0, 0.18, 1);
  -moz-transition: all 400ms cubic-bezier(0, 0, 0.18, 1);
  -o-transition: all 400ms cubic-bezier(0, 0, 0.18, 1);
  transition: all 400ms cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -moz-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -o-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  position: absolute;
  width: 100%;
  bottom: 25px;
}

.info-inner .p-name,
.info-inner .p-company {
  display: block;
}

.info-inner .p-name {
  font-family: 'Roboto', sans-serif;
  font-size: 18px;
  color: #252525;
}

.info-inner .p-company {
  font-family: 'Roboto', sans-serif;
  font-size: 12px;
  text-transform: uppercase;
  color: #8c8c8c;
}

.a-size {
  -webkit-transition: all 300ms cubic-bezier(0, 0, 0.18, 1);
  -moz-transition: all 300ms cubic-bezier(0, 0, 0.18, 1);
  -o-transition: all 300ms cubic-bezier(0, 0, 0.18, 1);
  transition: all 300ms cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -moz-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -o-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  position: absolute;
  width: 100%;
  bottom: -20px;
  font-family: 'Roboto', sans-serif;
  color: #828282;
  opacity: 0;
}

.a-size .size {
  color: #252525;
}

.cart {
  display: block;
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  font-family: 'Roboto', sans-serif;
  font-weight: 700;
}

.cart .price {
  -webkit-transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  -moz-transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  -o-transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -moz-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -o-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-delay: 100ms;
  -o-transition-delay: 100ms;
  transition-delay: 100ms;
  display: block;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  -o-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  font-size: 16px;
  color: #252525;
}

.cart .add-to-cart {
  -webkit-transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  -moz-transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  -o-transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  transition: all 600ms cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -moz-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  -o-transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  transition-timing-function: cubic-bezier(0, 0, 0.18, 1);
  /* ease-out */
  -webkit-transition-delay: 100ms;
  -o-transition-delay: 100ms;
  transition-delay: 100ms;
  display: block;
  position: absolute;
  top: 50%;
  left: 110%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  -o-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}

.cart .add-to-cart .txt {
  font-size: 12px;
  color: #fff;
  letter-spacing: 0.045em;
  text-transform: uppercase;
  white-space: nowrap;
}


.ecom_offer{
  font-family: 'Roboto', sans-serif;
}
.ecom_offer .ecom_h4{
  font-size: 36px;
  font-weight: 700;
  font-family: 'Raleway', sans-serif;
  margin-bottom: 20px;
  display: inline-block;
}
.ecom_offer .ecom_p{
  font-size: 18px;
  float: right;
  font-family: 'Raleway', sans-serif;
  margin-bottom: 20px;
}
@media(max-width: 991px){
  .ecom_offer .ecom_h4{
    font-size: 25px;
    font-weight: 500;
    font-family: 'Raleway', sans-serif;
  }
}
.ecom_offer .swiper-slide{
  width: 654px !important;
  margin-right: 20px;
}
.wrapper {
  height: 420px;
  width: 654px;
}
.product-img {
  float: left;
  height: 420px;
  width: 327px;
}
.product-img img {
  border-radius: 7px 0 0 7px;
}
.product-info {
  float: left;
  height: 420px;
  width: 327px;
  border-radius: 0 7px 10px 7px;
  background-color: #ffffff;
}
.product-text {
  height: 250px;
  width: 327px;
}
.product-text h1 {
  margin: 0 0 0 38px;
  padding-top: 52px;
  font-size: 34px;
  color: #474747;
}
.product-text h1,
.product-price-btn p {
  font-family: 'Roboto', serif;
}
.product-text p {
  height: 125px;
  width: 245px;
  margin: 0 0 0 38px;
  font-family: 'Roboto', serif;
  color: #8d8d8d;
  line-height: 1.7em;
  font-size: 15px;
  font-weight: lighter;
  overflow: hidden;
}
.ecom_offer span {
  display: inline-block;
  height: 50px;
  font-family: 'Roboto', serif;
  font-size: 34px;
}

.product-price-btn button {
  display: inline-block;
  height: 50px;
  width: 176px;
  margin: 0 40px 18px 40px;
  box-sizing: border-box;
  border: transparent;
  border-radius: 60px;
  font-family: 'Raleway', sans-serif;
  font-size: 14px;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: #ffffff;
  background-color: #9cebd5;
  cursor: pointer;
  outline: none;
}
.product-price-btn button:hover {
  background-color: #79b0a1;
}
@media(max-width: 991px){
  .ecom_offer .swiper-slide{
    width: 270px !important;
  }
  .wrapper {
    height: 105px;
    width: 250px;
  }
  .product-img {
    float: left;
    height: 250px;
    width: 100px;
    align-items: center;
  }
  .product-img img {
    border-radius: 7px 0 0 7px;
    width: 270px;
    height: 100%;
    object-fit: cover;
  }
  .product-info {
    height: 200px;
    width: 270px;
    border-radius: 0 7px 10px 7px;
    background-color: #ffffff;
  }
  .product-text {
    height: 120px;
    width: 327px;
  }
  .product-text h1 {
    margin: 0 0 0 38px;
    padding-top: 7px;
    font-size: 25px;
    color: #474747;
  }
  .product-text h1,
  .product-price-btn p {
    font-family: 'Roboto', serif;
  }
  .product-text p {
    height: 70px;
    width: 180px;
    margin: 0 0 0 38px;
    font-family: 'Roboto', serif;
    color: #8d8d8d;
    line-height: 1.7em;
    font-size: 11px;
    font-weight: lighter;
    overflow: hidden;
  }
  .product-price-btn button {
    display: inline-block;
    height: 25px;
    width: 88px;
    margin: 0 40px 0px 40px;
    box-sizing: border-box;
    border: transparent;
    border-radius: 60px;
    font-family: 'Raleway', sans-serif;
    font-size: 7px;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 0.2em;
    color: #ffffff;
    background-color: #9cebd5;
    cursor: pointer;
    outline: none;
  }
  .product-price-btn button:hover {
    background-color: #79b0a1;
  }
}
</style>
