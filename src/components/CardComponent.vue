<template>
<div>
      <div class="img_box">
    <img :src="thumb" :alt="titolo" />
  </div>
  <div>
    <h5>{{ title }}</h5>
  </div>

</div>

</template>

<script>
export default {
  nome: "CardComponent",
  props: {
    //pasta : Object,
    thumb: String,
    title: String,
  },
};
</script>

<style lang="scss" scoped>
.img_box {
        aspect-ratio: 1/1;
        overflow: hidden;
        margin-bottom: 1rem;
        img {
          width: 100%;
        }
      }

      h5 {
        color: $dc-light;
      }
</style>
