<template lang="html">
  <div class="footer">
    <footer class="background">
      <div class="container ecom_footer">
        <div class="row mb-5">
          <div class="col-lg-2 col-md-6">
            <p class="text-left text_footer">Top Products</p>
            <ul>
              <li>
                <a href="">
                  Manage Websites
                </a>
              </li>
              <li>
                <a href="">
                  Manage Relations
                </a>
              </li>
              <li>
                <a href="#">
                  Power Tools
                </a>
              </li>
              <li>
                <a href="#">
                  Marketing Service
                </a>
              </li>
            </ul>
          </div>
          <div class="col-lg-2 col-md-6">
            <p class="text-left text_footer">Quick Links</p>
            <ul>
              <li><a href="">Jobs</a></li>
              <li><a href="">Brand Assets</a></li>
              <li><a href="#">Investor Relations</a></li>
              <li><a href="#">Terms Of Service</a></li>
            </ul>
          </div>
          <div class="col-lg-2 col-md-6">
            <p class="text-left text_footer">Features</p>
            <ul>
              <li><a href="">Jobs</a></li>
              <li><a href="">Brand Assets</a></li>
              <li><a href="#">Investor Relations</a></li>
              <li><a href="#">Terms Of Service</a></li>
            </ul>
          </div>
          <div class="col-lg-2 col-md-6">
            <p class="text-left text_footer">Resources</p>
            <ul>
              <li><a href="">Guides</a></li>
              <li><a href="">Research</a></li>
              <li><a href="#">Experts</a></li>
              <li><a href="#">Agencies</a></li>
            </ul>
          </div>
          <div class="col-lg-4 col-md-12">
            <h2 class="text-left text_footer">About Us</h2>
            <p class="text-left text_footer_p">
              We offer superior customer service to the wide base of our clients. Our business-driven approach separates us from typical Website Design Companies.We have built a reputation for creating a positive return on investment our clients.
            </p>
          </div>
        </div>
        <div class="row mt-5">
          <div class="col-md-12 col-lg-8">
            <p class="text-left text_footer">© 2020 Ecommerce. All rights reserved Under Ecommerce.</p>
          </div>
          <div class="col-md-12 col-lg-4 footer_social text-left">
            <a href="#">
              <i class="fa fa-facebook"></i>
            </a>
            <a href="#">
              <i class="fa fa-instagram"></i>
            </a>
            <a href="#">
              <i class="fa fa-linkedin"></i>
            </a>
            <a href="#">
              <i class="fa fa-twitter"></i>
            </a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "footer"
}
</script>

<style lang="css" scoped>
.background
{
	background-image: linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.9));
  background-position: center;
  background-size: cover;
}
.ecom_footer{
	padding-top: 140px;
	padding-bottom: 90px;
}
.ecom_footer .text_footer{
	font-size: 18px;
	text-decoration: none;
	color: #ffffff;
	font-weight: 900;
	font-family: 'Raleway', sans-serif;
	margin-bottom: 25px;
}
.ecom_footer ul a{
	color: #ffffff;
}
.ecom_footer ul{
  padding-left: 0px;
}
.ecom_footer ul li{
  list-style: none;
	font-size: 14px;
	line-height: 41px;
	font-family: 'Roboto', serif;
}
.text_footer_p{
	line-height: 25px;
	font-size: 14px;
	margin-top: 36px;
	font-family: 'Roboto', serif;
	letter-spacing: 1px;
	color: #ffffff;
}
.ecom_footer .footer_social{
	text-align: center;
}
.ecom_footer .footer_social a{
	padding: 7px 11px;
	border-radius: 2px;
	background: #ffffff;
	margin: 11px;
	text-align: center;
	text-decoration: none;
}
@media(max-width: 991px){
	.ecom_footer .text_footer{
		margin-top: 45px;
		margin-bottom: 15px;
	}
	.ecom_footer .footer_social{
		margin-top: 25px;
		text-align: center;
	}
}
</style>
