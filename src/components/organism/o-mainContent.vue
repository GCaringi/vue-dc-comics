<template>
    <main>
        <jumbo/>
        <div class = "m-gallery__wrapper">
            <gallery/>
        </div>
    </main>
</template>

<script>

import jumbo from '../molecules/m-jumbotron.vue'
import gallery from '../molecules/m-gallery.vue'

export default {
    name: "mainCs",
    components: {
        jumbo,
        gallery,
    }
}
</script>

<style lang = "scss" scoped>

    .m-gallery__wrapper{
        width: 100%;
        background-color: var(--clr-secondary);
    }
</style>