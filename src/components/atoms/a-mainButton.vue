<template>
  <button class = "btn_cs">
      {{text}}
  </button>
</template>

<script>
export default {
    name: "mainBtn",
    props: {
        text: {
            type: String,
            required: true,
        }
    }
}
</script>

<style lang = "scss" scoped>

.btn_cs{
    background-color: var(--clr-primary);
    border: none;
    color: var(--clr-base-light);
    text-transform: uppercase;
    font-size: var(--fs-xl);
    font-weight: var(--fw-xl);
    padding: var(--space-lg);
    cursor: pointer;
}

</style>