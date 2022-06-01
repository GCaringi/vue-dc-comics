<template>
  <div id="app" class="o-fullContainer" >
    <div class="o-pageContainer">
      <headerCs/>
    </div>
    <div class="wrapper__main">
      <div class="o-pageContainer">
        -->Content goes here...
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
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
  }

  .wrapper__main{
    background-color: var(--clr-secondary);
    color: var(--clr-base-light);
    width: 100%;
    height: var(--main-height);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: var(--fs-xxl);
    font-weight: bold;
    // padding-top: var(--space-xxxl);
    // padding-bottom: var(--space-xxxl);
  }

  .o-pageContainer{
    // display: flex;
    // justify-content: center;
    width: var(--width-xl);
  }
</style>
