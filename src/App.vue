<template>
  <div id="app">
    <headerBar/>
    <mainContent/>
    <footerBar/>
  </div>

</template>

<script>
import headerBar from './components/organism/o-header.vue';
import mainContent from './components/organism/o-mainContent.vue'
import footerBar from './components/organism/o-footer.vue'

export default {
  name: 'App',
  components: {
    headerBar,
    mainContent,
    footerBar
  }
}
</script>

<style lang="scss">
  @import "./assets/style/global.scss";
  
</style>
