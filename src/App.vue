<template>
  <div id="app">
    <div class="wrapper">
      <HeaderSite />
      <MainSite></MainSite>
      <FooterSite></FooterSite>
    </div>
  </div>
</template>

<script>
import HeaderSite from "@/components/HeaderComponent.vue";
import MainSite from "@/components/MainSiteComponent.vue";

import FooterSite from "@/components/FooterComponent.vue";

export default {
  name: "App",
  components: {
    HeaderSite,
    MainSite,
    FooterSite,

  },
};
</script>

<style lang="scss">
@import "~@/assets/scss/style.scss";
</style>
