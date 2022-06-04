<template>
  <div class = "a-icons">
      <!-- TODO: Insert image dinamically -->
      <img src="" alt = "test">
      <h5>{{text}}</h5>
  </div>
</template>

<script>
export default {
    name: "FooterIcons",
    props: {
      srcs: {
        type: String,
        required: true,
      },
      text: {
        type: String,
      }
    }
}
</script>

<style lang = "scss" scoped>
    .a-icons{
      display: flex;
      align-items: center;
    }
        img{
          width: 50px;
          height: 70px;
        }
        h5{
          color: var(--clr-base-light);
          padding-left: var(--space-sm);
          text-transform: uppercase;
          font-size: var(--fs-md);
        }
</style>