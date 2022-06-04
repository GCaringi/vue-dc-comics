<template>
    <h4>{{head}}</h4>
</template>

<script>
export default {
    name: "listTitle",
    props: ["head"]
}
</script>

<style lang = "scss" scoped>

    h4{
        text-transform: uppercase;
        
        color: var(--clr-base-light);
    }

</style>