<template>
  <div id="app">
    <headerBar/>
    <div class="wrapper__main">
      <mainContent/>
    </div>
  </div>

</template>

<script>
import headerBar from './components/organism/o-header.vue';
import mainContent from './components/organism/o-mainContent.vue'

export default {
  name: 'App',
  components: {
    headerBar,
    mainContent,
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
