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
                <div class="row links_bar">
                  <div class="col">
                    <ul>
                      <li>
                        <h3>{{ footerLinks[0].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[0].details" :key="link">
                        <span>{{ link }}</span>
                      </li>
                    </ul>
                    <ul>
                      <li>
                        <h3>{{ footerLinks[1].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[1].details" :key="link">
                        <span>{{ link }}</span>
                      </li>
                    </ul>
                  </div>
                  <div class="col">
                    <ul>
                      <li>
                        <h3>{{ footerLinks[2].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[2].details" :key="link">
                        <span>{{ link }}</span>
                      </li>
                    </ul>
                  </div>
                  <div class="col">
                    <ul>
                      <li>
                        <h3>{{ footerLinks[3].title }}</h3>
                      </li>
                      <li v-for="link in footerLinks[3].details" :key="link">
                        <span>{{ link }}</span>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
              <div class="col">
                <img class="logo_bg" src="@/assets/img/dc-logo-bg.png" alt="" />
              </div>
            </div>
          </div>
        </div>
        <div class="footer_banner">
          <div class="container">
            <div class="row">
              <div class="col">
                <button><h3>Sign Up Now</h3></button>
              </div>
              <div class="col">
                <img
                  src="@/assets/img/footer-facebook.png"
                  alt="facebook icon"
                />
                <img src="@/assets/img/footer-twitter.png" alt="twitter icon" />
                <img src="@/assets/img/footer-youtube.png" alt="youtube icon" />
                <img
                  src="@/assets/img/footer-pinterest.png"
                  alt="pinterest icon"
                />
                <img
                  src="@/assets/img/footer-periscope.png"
                  alt="periscope icon"
                />
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
    .container > .row {
      height: 28rem;
      align-items: center;
      .col {
        color: white;
        text-transform: uppercase;
        text-align: start;
        margin-right: 1rem;
        .links_bar {
          align-items: flex-start;
        }

        ul li {
          margin-bottom: 0.2rem;
          span {
            opacity: 0.5;
            font-size: 0.7rem;
          }
          h3 {
            opacity: unset;
          }
        }
      }
    }
  }
  .footer_banner {
    background-color: #303030;
    padding: 2rem;
    .row {
      justify-content: space-between;

      .col img{
        padding: 0 0.8rem;
      }
      button{
        border: unset;
        color: white;
        padding: 1rem;
        background-color: unset;
        border: 2px solid #0282f9;

      }
    }
  }
}
</style>
