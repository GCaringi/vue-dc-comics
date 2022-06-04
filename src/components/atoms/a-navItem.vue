<template>
    <li class = "a-navItem" :class = "{'active' : isActive}">
        <a href="#">{{info}}</a>
    </li>
</template>

<script>
export default {
    name: "listItem",
    props: {
        info: {
            type: String,
            required: true,
        },
        isActive:{
            type: Boolean,
        }
    }
}
</script>

<style lang = "scss" scoped>
    .a-navItem{
        list-style: none;
        position: relative;
    }
        a{
            color: inherit;
            text-decoration: none;
            text-transform: uppercase;
            font-size: var(--fs-md);
            font-weight: var(--fw-lg);
            cursor: pointer;
        }
    .a-navItem.active{
        color: var(--clr-primary);
    }
    
    .active::after{
        position: absolute;
        content: "";
        width: 100%;
        height: var(--active-element-height);
        background-color: var(--clr-primary) ;
        top: calc(var(--header-height) / 2 - var(--space-lg) );
        left: 0px;
    }
</style>