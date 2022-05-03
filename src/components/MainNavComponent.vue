<template>
            <div class="main_navigation">
          <div class="container">
            <div class="row">
              <div class="col">
                <img src="@/assets/img/buy-comics-digital-comics.png" alt="" />
                <h5>digitals comics</h5>
              </div>
              <div class="col">
                <img src="@/assets/img/buy-comics-merchandise.png" alt="" />
                <h5>dc merchandises</h5>
              </div>
              <div class="col">
                <img src="@/assets/img/buy-comics-subscriptions.png" alt="" />
                <h5>subscription</h5>
              </div>
              <div class="col">
                <img src="@/assets/img/buy-comics-shop-locator.png" alt="" />
                <h5>comic shop locator</h5>
              </div>
              <div class="col">
                <img src="@/assets/img/buy-dc-power-visa.svg" alt="" />
                <h5>dc power visa</h5>
              </div>
            </div>
          </div>
        </div>
</template>
<script>
export default {
    name:"MainNav"
}
</script>

<style lang="scss" scoped>

  .main_navigation {
    background-color: #0282f9;
    .row {
      justify-content: space-around;
      padding: 2rem;

      .col{
        display: flex;
        align-items: center;
      }

      .col img{
        height: 4rem; 
        margin: 0 1rem;
      }
      .col h5{
        text-transform: uppercase;
        padding-left: 0.2rem;
        color:white;
      }
    }
  }

</style>