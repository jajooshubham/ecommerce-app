<template lang="html">
  <div class="blog">
    <section>
      <div class="container-fluid background">
        <div class="container">
          <div class="row">
            <div class="col-md-3"></div>
            <div class="col-md-6">
              <h3 class="text-center slide_text">Blogs</h3>
            </div>
            <div class="col-md-3"></div>
          </div>
        </div>
      </div>
    </section>


  </div>
</template>

<script>
export default {
  name: "blog",
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
</style>
