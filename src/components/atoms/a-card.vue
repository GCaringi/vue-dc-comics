<template>
  <div class="a-card">
    <img :src = imgUrl alt="">
  </div>
</template>

<script>
export default {
    name: "cardComics",
    props: {
      imgUrl: {
        type: String,
      }
    }
}
</script>

<style lang = "scss" scoped >
  .a-card{
    display: flex;
    justify-content: center;
    width: calc((100% / 6) - 10px);
  }
</style>