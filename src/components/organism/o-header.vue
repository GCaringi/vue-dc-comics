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
    name: "headerBar",
    components: { 
        logo,
        navBar,
    },
}
</script>

<style>
    .o-header{
        background-color: white;
        max-width: var(--width-xl);
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>