<template>
  <header id="header_site" class="container">
    <div class="row">
      <div class="site_logo">
        <img src="@/assets/img/dc-logo.png" alt="logo DC" />
      </div>
      <nav class="nav_site">
        <ul class="row">
          <li
            @click="activeIndex = index"
            :class="activeIndex === index ? 'active' : ''"
            v-for="(item, index) in navItems"
            :key="index"
            class="col">
            <a href="#">{{ item }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderSite",
  data() {
    return {
      activeIndex: 0,
      navItems: [
        "characters",
        "comics",
        "movies",
        "tv",
        "games",
        "collectibles",
        "videos",
        "fans",
        "news",
        "shop",
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
header {
  .site_logo img {
    width: 80px;
    padding: 0.6rem;
  }
  nav {
    background-color: $dc-light;
    height: 80px;
    display: flex;
    align-items: center;
    ul {
      list-style: none;
      height: 100%;
    }
    li {
      display: flex;
      align-items: center;
      height: 100%;
      font-size: 0.8rem;
      padding: 0 1rem;
      font-weight: bold;
      text-transform: uppercase;
      padding-bottom: 0.2rem;
    }
    .active, li:hover{
      color: $dc-primary;
      border-bottom: 3px solid $dc-primary;
      margin-bottom: -3px;
    }
    .active a, li:hover a{
      color:  $dc-primary;
    }
  }
}
</style>