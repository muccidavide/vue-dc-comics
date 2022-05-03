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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-family: "Montserrat", sans-serif;
}

/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  max-width: 100%;
}

li {
  list-style: none;
}

.container {
  width: 80%;
  max-width: 1440px;
  margin: auto;
}

.row {
  display: flex;
  flex-wrap: nowrap;
  justify-content: space-between;
  align-items: center;
}

/* Main*/
/* Products */
.products {
  height: 150px;
  background-color: black;
}


</style>
