<template lang="html">
  <div class="contact">
    <section>
      <div class="container-fluid background">
        <div class="container">
          <div class="row">
            <div class="col-md-3"></div>
            <div class="col-md-6">
              <h3 class="text-center slide_text">Contact</h3>
            </div>
            <div class="col-md-3"></div>
          </div>
        </div>
      </div>
    </section>
    <section class="contact mt-2">
      <div class="container mb-5">
        <div class="row">
          <div class="col-lg-8">
            <div class="mb-4">
              <p class="ecom_contact_p">
                Get in Touch
              </p>
            </div>
            <div>
              <div>
                <form class="mt-1">
                  <div class="form-row">
                    <div class="form-group col-md-6">
                      <input type="text" class="form-control" placeholder="First Name">
                    </div>
                    <div class="form-group col-md-6">
                      <input type="email" class="form-control" placeholder="E-Mail">
                    </div>
                  </div>
                  <div class="form-row">
                    <div class="form-group col-md-12">
                      <input type="text" class="form-control" placeholder="Subject">
                    </div>
                  </div>
                  <div class="form-row">
                    <div class="form-group col-md-12">
                      <textarea placeholder="Your Message" rows="10" class="form-control">
                      </textarea>
                    </div>
                  </div>
                  <button type="submit" class="button4">Send Message</button>
                </form>
              </div>
            </div>
          </div>
          <div class="col-lg-4">
            <div class="mb-4">
              <p class="ecom_contact_p">
                Contact Us
              </p>
            </div>
            <div>
              <div class=" contact_info">
                <div class="row">
                  <div class="col-2">
                    <span class="size">
                      <i class="fa fa-home"></i>
                    </span>
                  </div>
                  <div class="col-10">
                    <p class="ecom_font_m mb-0">Ratanada, Jodhpur.</p>
                    <p class="ecom_font">Near Apex School, 342011</p>
                  </div>
                </div>
                <div class="row mt-2">
                  <div class="col-2">
                    <span class="size">
                      <i class="fa fa-mobile"></i>
                    </span>
                  </div>
                  <div class="col-10">
                    <p class="ecom_font_m mb-0">+91 722 981 4000</p>
                    <p class="ecom_font">Mon to Sun 9AM to 9PM</p>
                  </div>
                </div>
                <div class="row mt-2">
                  <div class="col-2">
                    <span class="size">
                      <i class="fa fa-envelope"></i>
                    </span>
                  </div>
                  <div class="col-10">
                    <p class="ecom_font_m mb-0">ecom@ecommerce.com</p>
                    <p class="ecom_font">Near Apex School, 342011</p>
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
export default {
  name: "contact"
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
.ecom_contact_p{
  margin: 14px 0px 5px 0px;
  letter-spacing: 2px;
  font-size: 25px;
  font-weight: 900px;
}
.button4
{
	line-height: 25px;
	background: #2c75ba;
	color: #fff;
	border: 2px solid #2c75ba;
	border-radius: 2px;
  padding: 9px;
}
.ecom_font_m{
  font-size: 20px;
}
.ecom_font{
  font-size: 16px;
  font-weight: lighter;
  text-decoration-color: #fafafa;
}
.size{
  font-size: 25px;
}
i{
  width: 45px;
  height: 25px;
}
</style>
