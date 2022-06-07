<template>
  <div class = "container">
    <button-main class = "btn_cs__absolute"
    text = "Current Series"
    />
    <div class = "m-gallery__wrapper">
      <card
      v-for = "(element, index) in myData"
      :key = "index"
      :imgUrl = "element.thumb"
      :imgName = "element.series"
      />
    </div>
    <div class = "btn__wrapper">
      <button-main
      text = "Load More..."
      />
    </div>
  </div>
</template>

<script>

import buttonMain from '../atoms/a-mainButton.vue'
import card from '../atoms/a-card.vue'
import jdata from '../../assets/data/dc-comics.json'

export default {
    name: "galleryImgs",
    data(){
      return {
        myData : jdata,
      }
    },
    components: {
        card,
        buttonMain,
    }
}
</script>

<style lang = "scss" scoped>

  .m-gallery__wrapper{
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    padding: calc(var(--space-largest) * 2) 0px;
    color: var(--clr-base-light);
    text-transform: uppercase;
    text-align: center;
    font-weight: var(--fw-lg);
  }

  .container{
    max-width: var(--width-xl);
    margin: auto;
    position: relative;
  }

  .btn_cs__absolute{
    position: absolute;
    top: 0px;
    left: 0px;
    transform: translateY(-50%);
  }

  .btn__wrapper{
    text-align: center;
    padding-bottom: var(--space-largest);
  }

</style>