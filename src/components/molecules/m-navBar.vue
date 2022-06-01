<template>
  <ul class = "m-navbar">
    <listItem/>
    <listItem/>
    <listItem/>
    <listItem/>
    <listItem/>
    <listItem/>
    <listItem/>
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

<style lang = "scss" scoped>
    .m-navbar{
        position: relative;
        display: flex;
        column-gap: var(--space-xl);
        padding: var(--space-sm);
    }
</style>