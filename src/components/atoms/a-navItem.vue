<template>
    <li class = "a-navItem">
        <a class = "active" href="#">Prova</a>
    </li>
</template>

<script>
export default {
    name: "listItem"
}
</script>

<style lang = "scss" scoped>
    .a-navItem{
        position: relative;
        list-style: none;
    }
        a{
            color: inherit;
            text-decoration: none;
            text-transform: uppercase;
            font-size: var(--fs-md);
            font-weight: var(--fw-lg);
            cursor: pointer;
        }
    a:hover::after{
        content: "";
        position: absolute;
        background-color: var(--clr-primary) ;
        width: 100%;
        height: 5px;
        top: calc(var(--header-height) / 2 - 12px);
        left: 0px;
    }
</style>