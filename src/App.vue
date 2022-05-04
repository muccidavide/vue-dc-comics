<template>
  <div id="app">
    <div class="wrapper">
      <HeaderSite />

      <main id="main_site">
        <div class="products"></div>
        <MainNav></MainNav>
      </main>
      <FooterSite></FooterSite>

    </div>
  </div>
</template>

<script>

import HeaderSite from "@/components/HeaderComponent.vue";
import MainNav from "@/components/MainNavComponent.vue";
import FooterSite from "@/components/FooterComponent.vue";
export default {
  name: "App",
  components: {
    HeaderSite,
    MainNav,
    FooterSite,
  },

};
</script>

<style lang="scss">
 @import '~@/assets/scss/style.scss'; 

.products {
  height: 150px;
  background-color: $dc-dark;
}


</style>
