<template>
    <footer>
        <topFooter/>
        <middle-footer/>
        <bottom-footer/>
    </footer>
</template>

<script>

import topFooter from '../molecules/m-topFooter.vue'
import middleFooter from '../molecules/m-middleFooter.vue'
import bottomFooter from '../molecules/m-bottomFooter.vue'

export default {
    name : "FooterBar",
    components: {
        topFooter,
        middleFooter,
        bottomFooter,
    }
}
</script>

<style>

</style>