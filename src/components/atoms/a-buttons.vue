<template>
  <button class = "a-btn_cs">
      SIGN-UP NOW
  </button>
</template>

<script>
export default {
    name : "signUpBtn"
}
</script>

<style lang = "scss" scoped>

    .a-btn_cs{
        background-color: transparent;
        border: var(--space-xxxs) solid var(--clr-primary);
        padding: var(--space-xl) var(--space-xxl);
        color: var(--clr-base-light);
        font-size: var(--fs-lg);
        font-weight: var(--fw-xl);
        cursor: pointer;
    }
</style>