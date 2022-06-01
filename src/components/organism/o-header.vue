<template>
  <header class = "o-header">
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
    .o-header{
        background-color: white;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>