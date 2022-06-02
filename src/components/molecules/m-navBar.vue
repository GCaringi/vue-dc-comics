<template>
<nav>
  <ul class = "m-navbar">
    <list-item
      v-for= "(link,index) in links" 
      :key = "index" 
      :info = "link.text"
      :isActive = "link.active"
    />
  </ul>
</nav>
</template>

<script>

import listItem from '../atoms/a-navItem.vue'

export default {
    name: "navBar",
    components: {
        listItem,
    },
    data() {
        return {
            links : [
                {
                    text: "characters",
                    active: false,
                },
                {
                    text: "comics",
                    active: false,
                },
                {
                    text: "movies",
                    active: false,
                },
                {
                    text: "tv",
                    active: false,
                },
                {
                    text: "games",
                    active: false,
                },
                {
                    text: "collectibles",
                    active: true,
                },
                {
                    text: "video",
                    active: false,
                },
                {
                    text: "fans",
                    active: false,
                },
                {
                    text: "news",
                    active: false,
                },
                {
                    text: "shop",
                    active: false,
                },
            ]

        }
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