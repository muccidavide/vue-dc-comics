<template>
  <div id="app">
    <div class="wrapper">
      <HeaderSite />

      <main id="main_site">
        <div class="jumbotron">
          <img src="@/assets/img/jumbotron.jpg" alt="">
        </div>

        <MainProducts></MainProducts>
        <MainNav></MainNav>
      </main>
      <FooterSite></FooterSite>
    </div>
  </div>
</template>

<script>
import HeaderSite from "@/components/HeaderComponent.vue";
import MainProducts from "@/components/MainProductsComponent.vue"
import MainNav from "@/components/MainNavComponent.vue";
import FooterSite from "@/components/FooterComponent.vue";
export default {
  name: "App",
  components: {
    HeaderSite,
    MainNav,
    FooterSite,
    MainProducts
  },

};
</script>

<style lang="scss">
@import "~@/assets/scss/style.scss";

.jumbotron{
  height: 450px;
  overflow: hidden;
}
</style>
