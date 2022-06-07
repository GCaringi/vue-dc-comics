<template>
  <div class="m-jumbo">
  </div>
</template>

<script>
export default {
    name : "jumboImg"
}
</script>

<style lang = "scss" scoped>
    .m-jumbo{
        width: 100%;
        height: var(--jumbo-height);
        background-image: url("../../assets/img/jumbotron.jpg");
        background-size: cover;
        background-position: top center;
    }
</style>