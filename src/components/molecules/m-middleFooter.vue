<template>
  <div class="m-middleFooter">
      <div class="container">

      </div>
  </div>
</template>

<script>
export default {
    name: "middleFooter"
}
</script>

<style lang = "scss" scoped>
    .m-middleFooter{
        background-image: url("@/assets/img/footer-bg.jpg");
    }

    .container{
        margin: auto;
        width: var(--width-xl);
        height: 100%;
        display: flex;
        justify-content: flex-start;
        align-items: flex-start;
    }
</style>