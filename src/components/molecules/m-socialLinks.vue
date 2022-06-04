<template>
  <div class="m-socialLinks">
        <h5>Follow Us</h5>
        <ul>
            <li
            v-for = "(icons, index) in socialIcons"
            :key = "index"
            >
                <a href="#">
                    <img :src='require(`../../assets/img/${icons}`)' alt="prova">
                </a>
            </li>
        </ul>
  </div>
</template>

<script>
export default {
    name: "socialLinks",
    data(){
        return {
            socialIcons: [
                "footer-facebook.png",
                "footer-twitter.png",
                "footer-youtube.png",
                "footer-pinterest.png",
                "footer-periscope.png",
            ]
        }
    },
}
</script>

<style lang = "scss" scoped>
    .m-socialLinks{
        display: flex;
        align-items: center;
        column-gap: var(--space-md);
    }

    h5{
        text-transform: uppercase;
        color: var(--clr-primary);
        font-size: var(--fs-xl);
    }
    ul{
        list-style: none;
        display: flex;
        column-gap: var(--space-md);
    }
</style>