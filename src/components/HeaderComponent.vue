<template>
    <header id="header_site" class="row">
      <div class="site_logo">
        <img src="@/assets/img/dc-logo.png" alt="logo DC">
      </div>
      <nav class="nav_site">
        <ul class="row">
          <li v-for="item in navItems" :key="item" class="col">{{item}}</li>
        </ul>


      </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderSite',
    data(){
      return{
        navItems:['characters',
        'comics',
        'movies',
        'tv',
        'games',
        'collectibles',
        'videos',
        'fans',
        'news',
        'shop']
      }
    }
}
</script>
<style lang="scss" scoped>

</style>