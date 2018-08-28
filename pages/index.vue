<template lang="pug">
  .container
    Apphead
    // Pageheader
    Imageslide
    //Corossel
    Tile
    Banner1
    Footer
</template>
<script>
import Pageheader from '../components/pageheader.vue'
import Apphead from '../components/app-head.vue'
import Corossel from '../components/corossel.vue'
import Tile from "../components/tile.vue"
import Banner1 from "../components/banner1.vue"
import Footer from "../components/footer1.vue"
import Imageslide from "../components/imageslide.vue"
export default {
  components:{
    Pageheader,
    Corossel,
    Apphead,
    Tile,
    Banner1,
    Footer,
    Imageslide
  }
}
</script>
<style lang="sass" scoped>

</style>


