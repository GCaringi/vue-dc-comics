<template>
    <h4>{{head}}</h4>
</template>

<script>
export default {
    name: "listTitle",
    props: {
        head: {
            type:String,
            required: true
        }
    }
}
</script>

<style lang = "scss" scoped>

    h4{
        text-transform: uppercase;
        margin: 0px;
        color: var(--clr-base-light);
        font-size: var(--fs-xxl);
    }

</style>