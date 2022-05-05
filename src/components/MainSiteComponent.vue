<template>
      <main id="main_site">
        <JumbotronMain></JumbotronMain>
        <MainProducts></MainProducts>
        <MainNav></MainNav>
      </main>
  
</template>

<script>
import JumbotronMain from "@/components/JumbotronComponent.vue";
import MainProducts from "@/components/MainProductsComponent.vue";
import MainNav from "@/components/MainNavComponent.vue";

export default {
    components: {
    MainNav,
    JumbotronMain,
    MainProducts,
  },

}
</script>

<style>

</style>