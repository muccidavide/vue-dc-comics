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
            {{ item }}
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
  padding: 1.2rem;
  .site_logo img {
    width: 80px;
  }
  nav {
    background-color: white;
    height: 80px;
    display: flex;
    align-items: center;
    ul {
      list-style: none;
    }
    li {
      font-size: 0.8rem;
      padding: 0 1rem;
      font-weight: bold;
      text-transform: uppercase;
      padding-bottom: 0.2rem;
    }
    .active {
      color: #0282f9;
      border-bottom: 3px solid #0282f9;
    }
  }
}
</style>