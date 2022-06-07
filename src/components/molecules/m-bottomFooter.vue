<template>
    <div class="m-bottomFooter">
        <div class="container">
            <sign-btn/>
            <social-links/>
        </div>
    </div>
</template>

<script>

import signBtn from '../atoms/a-buttons.vue'
import socialLinks from './m-socialLinks.vue'

export default {
    name: "bottomFooter",
    components: {
        signBtn,
        socialLinks,
    }
}
</script>

<style lang = "scss" scoped>
    .m-bottomFooter{
        background-color: var(--clr-tertiary);
        padding-top: var(--space-largest);
        padding-bottom: var(--space-largest);
    }

    .container{
        max-width: var(--width-xl);
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }


</style>