<template>
  <div class = "container">
    <card
    v-for = "(element, index) in myData"
    :key = "index"
    :imgUrl = "element.thumb"
    />
  </div>
</template>

<script>

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
    }
}
</script>

<style lang = "scss" scoped>

  .container{
    width: var(--width-xl);
    margin: auto;
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }

</style>