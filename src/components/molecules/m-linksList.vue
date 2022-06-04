<template>
    <ul>
        <li 
        v-for = "(element, index) in obj.links" 
        :key = "index"
        >
            <a href="#">{{element}}</a>            
        </li>
    </ul>
</template>

<script>


export default {
    name: "linksList",
    props: {
        obj: {
            type: Object,
        }
    }
}
</script>

<style lang = "scss" scoped>
    ul{
        margin: 0px;
        list-style: none;
    }   
        a{
            font-size: var(--fs-lg) ;
            text-decoration: none;
            color: var(--clr-socialLinks);
            opacity: 0.7;
            cursor: pointer;
        &:hover{
            opacity: 1;
        }
    }

</style>