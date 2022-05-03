<template>
  <div id="app">
    <div class="wrapper">
      <HeaderSite />

      <main id="main_site">
        <div class="products"></div>
        <MainNav></MainNav>
      </main>
      <footer id="footer_site">
        <div class="footer_wrapper">
          <div class="container">
            <div class="row">
              <div class="col">
                <div class="row">
                  <div class="col">
                    <ul>
                      <li>
                        <h3>{{ footerLinks[0].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[0].details" :key="link">
                        {{ link }}
                      </li>
                    </ul>
                    <ul>
                      <li>
                        <h3>{{ footerLinks[1].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[1].details" :key="link">
                        {{ link }}
                      </li>
                    </ul>
                  </div>
                  <div class="col">
                    <ul>
                      <li>
                        <h3>{{ footerLinks[2].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[2].details" :key="link">
                        {{ link }}
                      </li>
                    </ul>
                  </div>
                  <div class="col">
                     <ul>
                      <li>
                        <h3>{{ footerLinks[2].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[2].details" :key="link">
                        {{ link }}
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
              <div class="col">
                <img class="logo_bg" src="@/assets/img/dc-logo-bg.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
import HeaderSite from "@/components/HeaderComponent.vue";
import MainNav from "@/components/MainNavComponent.vue";

export default {
  name: "App",
  components: {
    HeaderSite,
    MainNav,
  },
  data() {
    return {
      footerLinks: [
        {
          title: "dc comics",
          details: [
            "characters",
            "comics",
            "movies",
            "tv",
            "games",
            "collectibles",
            "videos",
            "news",
          ],
        },
        {
          title: "shop",
          details: ["Shop DC ", "Shop DC Collectibles"],
        },
        {
          title: "DC",
          details: [
            "Terms Of Use",
            "Privacy Policy(New)",
            "Ad Choices",
            "Advertising",
            "Jobs",
            "Subscriptions",
            "Talent Workshop",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us",
          ],
        },
        {
          title: "Sites",
          details: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa",
          ],
        },
      ],
    };
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
  margin-top: 1rem;
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

footer {
  .footer_wrapper {
    background: url("@/assets/img/footer-bg.jpg");
    overflow: hidden;
    background-size: cover;
    background-repeat: no-repeat;

  }
  .row {
        height: 25rem;
    .col {
      color: white;
      text-transform: uppercase;
      ul h3 {
        font-size: 1.5rem;
      }
      ul li {
        font-size: 0.8rem;
      }
    }
  }
}
</style>
