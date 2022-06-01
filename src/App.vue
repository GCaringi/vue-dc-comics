<template>
  <div id="app" class="o-fullContainer" >
    <div class="o-pageContainer">
      <headerCs/>
    </div>
  </div>
</template>

<script>
import headerCs from './components/organism/o-header.vue';

export default {
  name: 'App',
  components: {
    headerCs,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/global.scss";
  .o-fullContainer{
    width: 100%;
    display: flex;
    justify-content: center;
  }

  .o-pageContainer{
    display: flex;
    justify-content: center;
    width: var(--width-xl);
  }
</style>
