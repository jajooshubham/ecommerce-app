<template lang="html">
  <div class="header">
    <header>
      <nav class="navbar navbar-expand-lg navbar-light bg-light fixed-top scrolling-navbar">
        <div class="container">

          <a class="navbar-brand" href="">
            <img src="@/assets/logo.png">
          </a>

          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#basicExampleNav"
          aria-controls="basicExampleNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="basicExampleNav">

          <ul class="navbar-nav ml-auto">

            <li class="nav-item">
              <router-link to="/" class="nav-link waves-effect">Home</router-link>
            </li>

            <li class="nav-item">
              <router-link to="/about" class="nav-link waves-effect">About</router-link>
            </li>

            <li class="nav-item">
              <router-link to="" class="nav-link waves-effect">Products</router-link>
            </li>

            <li class="nav-item">
              <router-link to="/blog" class="nav-link waves-effect">Blog</router-link>
            </li>

            <li class="nav-item">
              <router-link to="/contact" class="nav-link waves-effect">Contact</router-link>
            </li>

            <li class="nav-item">
              <router-link to="/sign-in" class="nav-link waves-effect">Sign In</router-link>
            </li>

            <li class="nav-item mb-2 mb-md-0">
              <router-link to="/register" type="button" class="btn btn-outline-info btn-md btn-rounded btn-navbar waves-effect waves-light">Register</router-link>
            </li>

            <li class="nav-item">
              <router-link to="/search" class="nav-link navbar-link-2 waves-effect">
                <i class="fa fa-search pl-0 ml-3"></i>
              </router-link>
            </li>
            <li class="nav-item">
              <a href="#!" class="nav-link navbar-link-2 waves-effect">

                <i class="fa fa-shopping-cart pl-0 ml-3"></i>
              </a>
            </li>
            <li class="nav-item">
              <a href="#!" class="nav-link navbar-link-2 waves-effect">

                <i class="fa fa-heart pl-0 ml-3"></i>
              </a>
            </li>

          </ul>

        </div>
      </div>
    </nav>
  </header>
  </div>
</template>

<script>
export default {
  name: "header"
}
</script>

<style lang="css" scoped>
</style>
