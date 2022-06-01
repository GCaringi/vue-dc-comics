<template>
  <header>
      <logo/>
      <nav-bar/>
  </header>
</template>

<script>
import logo from '../atoms/a-logo.vue'
import navBar from '../molecules/m-navBar.vue'

export default {
    name: "HeadBar",
    components: { 
        logo,
        navBar,
    },
}
</script>

<style>
    header{
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-content: center;
    }
</style>