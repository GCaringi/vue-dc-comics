<template>
  <div class="m-topFooter">
      <div class="container">
        <iconsTop/>
        <iconsTop/>
        <iconsTop/>
        <iconsTop/>
        <iconsTop/>
      </div>
  </div>
</template>

<script>

import iconsTop from '../atoms/a-icons.vue'

export default {
    name: "topFooter",
    components: {
        iconsTop,
    }
}
</script>

<style lang = "scss" scoped>
    .m-topFooter{
        background-color: var(--clr-primary);
        height: var(--topFooter-height);
        
    }

    .container{
        margin: auto;
        width: var(--width-xl);
        height: 100%;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
</style>