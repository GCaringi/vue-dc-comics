<template>
    <footer>
        <topFooter/>
        <middle-footer/>
    </footer>
</template>

<script>

import topFooter from '../molecules/m-topFooter.vue'
import middleFooter from '../molecules/m-middleFooter.vue'

export default {
    name : "FooterBar",
    components: {
        topFooter,
        middleFooter,
    }
}
</script>

<style>

</style>