<template>
  <div class="main_navigation">
    <div class="container">
      <div class="row">
        <div class="col" v-for="item in banner" :key="item.id">
          <img :src="item.src" :alt="item.text" />
           <h5>{{item.text}}</h5>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
    name:"MainNav",
    data(){
      return{
        banner:[
          {
          id:1,
          src: require('@/assets/img/buy-comics-digital-comics.png'),
          text: 'digitals comics',
          },
                    {
          id:2,
          src: require('@/assets/img/buy-comics-merchandise.png'),
          text: 'dc merchandises',
          },
                    {
          id:3,
          src: require('@/assets/img/buy-comics-subscriptions.png'),
          text: 'subscription',
          },
                    {
          id:4,
          src: require('@/assets/img/buy-comics-shop-locator.png'),
          text: 'comic shop locator',
          },
                    {
          id:5,
          src: require('@/assets/img/buy-dc-power-visa.svg'),
          text: 'dc power visa',
          },

        ]
      }
      
    }
}
</script>

<style lang="scss" scoped>
.main_navigation {
  background-color: #0282f9;
  .row {
    justify-content: space-around;
    padding: 2rem;

    .col {
      display: flex;
      align-items: center;
    }

    .col img {
      height: 4rem;
      margin: 0 1rem;
    }
    .col h5 {
      text-transform: uppercase;
      padding-left: 0.2rem;
      color: white;
    }
  }
}
</style>