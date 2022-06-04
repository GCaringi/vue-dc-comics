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
        "obj" : Object,
    }
}
</script>

<style>

</style>