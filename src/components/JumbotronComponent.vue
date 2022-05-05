<template>
        <div class="jumbotron">
          <img src="@/assets/img/jumbotron.jpg" alt="">
        </div>
</template>
<script>

export default({
  name:"JumbotronMain",
})
</script>
<style lang="scss" scoped>
  
.jumbotron{
  height: 450px;
  overflow: hidden;
  img{
    object-fit: cover;
    width: 100%;
  }
}
</style>
