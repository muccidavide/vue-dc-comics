<template>
  <div id="app">
    <div class="wrapper">
      <HeaderSite/>
      
    <main id="main_site">

    </main>
    <footer id="footer_site">

    </footer>

    </div>
    
  </div>
</template>

<script>
import HeaderSite from '@/components/HeaderComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderSite,
  },
      
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 1rem;
  font-family: 'Montserrat', sans-serif;
}

/* Reset */
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img{
  max-width: 100%;
}

.wrapper{
  width: 80%;
  max-width: 1440px;
  margin: auto;
}

.row{
  display: flex;
  flex-wrap:nowrap;
  justify-content: space-between;
  align-items: center;
}

/* Header */
header{
  .site_logo img{
    width: 80px;
  }
  nav{
    background-color: white;
    height: 80px;
          display: flex;
      align-items: center;
    ul{
      list-style: none;

    }
    li{
      font-size: 0.8rem;
      padding: 0 1rem;
      font-weight: bold;
      text-transform: uppercase;
    }
  }
}




</style>
