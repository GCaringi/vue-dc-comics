<template>
  <div id="app" class="o-fullContainer" >
    <div class="o-pageContainer">
      <headerCs/>
    </div>
    <div class="wrapper__main">
      <div class="o-pageContainer">
        
      </div>
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
    //TODO: remove background color and 100vh
    width: 100%;
    height: 100vh;
    // background-color: black;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
  }

  .wrapper__main{
    width: 100%;
    background-color: var(--clr-secondary);
  }

  .o-pageContainer{
    // display: flex;
    // justify-content: center;
    width: var(--width-xl);
  }
</style>
