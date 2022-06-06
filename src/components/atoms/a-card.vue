<template>
  <div class="a-card">
    <img :src = imgUrl alt="">
    {{imgName}}
  </div>
</template>

<script>
export default {
    name: "cardComics",
    props: {
      imgUrl: {
        type: String,
        required: true,
      },
      imgName: {
        type: String,
      }
    }
}
</script>

<style lang = "scss" scoped>
  .a-card{
    display: flex;
    flex-direction: column;
    align-items: center;
    width: calc((100% / 6) - 10px);
    padding: var(--space-lg) 0px;
    cursor: pointer;
    img{
      width: 100%;
      padding-bottom: var(--space-lg);
    }
  }
</style>