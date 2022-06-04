<template>
  <div class="m-topFooter">
      <div class="container">
        <iconsTop
        v-for = "(element,index) in categories" 
        :key = "index"
        :srcs = "element.img"
        :text = "element.text"
        />
      </div>
  </div>
</template>

<script>

import iconsTop from '../atoms/a-icons.vue'

export default {
    name: "topFooter",
    components: {
        iconsTop,
    },
    data(){
        return {
            categories: [
                {
                    img: "buy-comics-digital-comics.png",
                    text: "digital comics"
                },
                {
                    img: "buy-comics-merchandise.png",
                    text: "dc merchandise"
                },
                {
                    img: "buy-comics-subscriptions",
                    text: "subscription"
                },
                {
                    img: "buy-comics-shop-locator.png",
                    text: "comic shop locator"
                },
                {
                    img: "buy-dc-power-visa.svg",
                    text: "dc power visa"
                },
            ]
        }
    }
}
</script>

<style lang = "scss" scoped>
    .m-topFooter{
        background-color: var(--clr-primary);
        height: var(--topFooter-height);
        
    }

    .container{
        margin: auto;
        width: var(--width-xl);
        height: 100%;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
</style>