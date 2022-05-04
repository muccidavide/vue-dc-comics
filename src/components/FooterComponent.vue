<template>
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
                    <a href="#">{{ link }}</a>
                  </li>
                </ul>
                <ul>
                  <li>
                    <h3>{{ footerLinks[1].title }}</h3>
                  </li>
                  <li v-for="link in footerLinks[1].details" :key="link">
                    <a href="#">{{ link }}</a>
                  </li>
                </ul>
              </div>
              <div class="col">
                <ul>
                  <li>
                    <h3>{{ footerLinks[2].title }}</h3>
                  </li>
                  <li v-for="link in footerLinks[2].details" :key="link">
                    <a href="#">{{ link }}</a>
                  </li>
                </ul>
              </div>
              <div class="col">
                <ul>
                  <li>
                    <h3>{{ footerLinks[3].title }}</h3>
                  </li>
                  <li v-for="link in footerLinks[3].details" :key="link">
                    <a href="#">{{ link }}</a>
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
            <img src="@/assets/img/footer-facebook.png" alt="facebook icon" />
            <img src="@/assets/img/footer-twitter.png" alt="twitter icon" />
            <img src="@/assets/img/footer-youtube.png" alt="youtube icon" />
            <img src="@/assets/img/footer-pinterest.png" alt="pinterest icon" />
            <img src="@/assets/img/footer-periscope.png" alt="periscope icon" />
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: "FooterSite",
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
<style lang="scss" scoped>
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
        color: $dc-light;
        text-transform: uppercase;
        text-align: start;
        margin-right: 1rem;
        .links_bar {
          align-items: flex-start;
        }

        ul li {
          margin-bottom: 0.1rem;
          a {
            color: $dc-light;
            opacity: 0.5;
            font-size: 0.7rem;
          }
          h3 {
            opacity: unset;
            margin: 1rem 0;
          }
        }
      }
    }
  }
  .footer_banner {
    background-color: $dc-dark;
    padding: 2rem;
    .row {
      justify-content: space-between;

      .col img {
        padding: 0 0.8rem;
      }
      button {
        @include button;
      }
    }
  }
}
</style>