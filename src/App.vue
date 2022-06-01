<template>
  <div id="app">
    <headerCs/>
    <div class="wrapper__main">
      <mainCs/>
    </div>
  </div>

</template>

<script>
import headerCs from './components/organism/o-header.vue';
import mainCs from './components/molecules/m-mainMy.vue'

export default {
  name: 'App',
  components: {
    headerCs,
    mainCs,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/global.scss";
  .wrapper__main{
    background-color: var(--clr-secondary);
    color: var(--clr-base-light);
    height: var(--main-height);
  }
</style>
