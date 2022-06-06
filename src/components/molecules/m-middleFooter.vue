<template>
  <div class="m-middleFooter">
      <div class="container">
          <div class = "lists" 
            v-for =  "(list, index) in lists"
            :key = "index"
            >
            <listTitle
                :head = "list.title"
            /> 
            <linksList
                :obj = "list" 
            />
          </div>
          <img class = "a-logo-bg" src="../../assets/img/dc-logo-bg.png" alt="">
      </div>
  </div>
</template>

<script>

import listTitle from '../atoms/a-listTitle.vue'
import linksList from '../molecules/m-linksList.vue'

export default {
    name: "middleFooter",
    components: {
        listTitle,
        linksList,
    },
    data(){
        return{
            lists: [
            {
                title: "dc Comics",
                links: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "TV",
                    "Games",
                    "Videos",
                    "News"
                ]
            },
            {
                title: "shop",
                links: [
                    "Shop DC",
                    "Shop DC Collectibles"
                ]
            },
            {
                title: "dc",
                links: [
                    "Terms Of Use",
                    "Privacy policy (New)",
                    "Ad choices",
                    "Advertising",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact Us"
                ]
            },
            {
                title: "sites",
                links: [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa"
                ]
            },

        ]
        }
    }
}
</script>

<style lang = "scss" scoped>
    .m-middleFooter{
        background-image: url("@/assets/img/footer-bg.jpg");
        background-size: cover;
        padding-top: var(--space-largest);
        padding-bottom: var(--space-largest);
        height: var(--middleFooter-height);
        overflow: hidden;
    }

    .container{
        width: var(--width-xl);
        height: inherit;
        margin: auto;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        align-content: flex-start;
        position: relative;
    }

    .lists{
        padding: var(--space-xxl) var(--space-xxl) var(--space-xxl) 0px;
    }

    .a-logo-bg{
        position: absolute;
        top: -30%;
        right: 0px;
    }

</style>