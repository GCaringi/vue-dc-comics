<template>
  <div class="m-middleFooter">
      <div class="container">

      </div>
  </div>
</template>

<script>



export default {
    name: "middleFooter",
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
    }

    .container{
        margin: auto;
        width: var(--width-xl);
        height: 100%;
        display: flex;
        justify-content: flex-start;
        align-items: flex-start;
    }
</style>