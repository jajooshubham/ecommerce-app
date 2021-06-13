<template>
  <div id="app">

    <perfect-scrollbar>

    <Header />
      <router-view />

    <Footer />
  </perfect-scrollbar>

  </div>
</template>

<script>
import Header from "@/components/Header"
import Footer from "@/components/Footer"
  export default{
    components: {
      Header,
      Footer
    }
  }
</script>

<style>
body{
    background-color: #e7f7f9;
    font-family: 'Roboto', sans-serif;
    position: relative;
}

.ps {
  height: 100vh;
}

.link {
  display: inline-block;
  padding: 10px;
}

</style>
