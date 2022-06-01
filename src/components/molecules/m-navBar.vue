<template>
  <ul class = "m-navbar">
      <li> <listItem/> </li>
      <li> <listItem/> </li>
      <li> <listItem/> </li>
      <li> <listItem/> </li>
  </ul>
</template>

<script>

import listItem from '../atoms/a-navItem.vue'

export default {
    name: "navBar",
    components: {
        listItem,
    }
}
</script>

<style>

</style>