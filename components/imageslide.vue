<template lang="pug">
.slideshow-container
  ul.slides
    li(v-for="(img, i) in images", :style="{ backgroundImage: `url(${img})` }", :class="{active: i === current}")
  .navigators
    button.prev(v-on:click="previous()") <
    button.next(v-on:click="next()") >
  .content
    h1 100% Organic
    p A new website template by 
      a(href='https://uicookies.com/') uicookies.com
    p under license 
      a(href='https://uicookies.com/license/') Creative Commons 3.0  
    button Get started
</template>

<script>
export default {
  data () {
    return {
      images: [
        'https://www.desktopbackground.org/download/2000x1500/2011/08/15/250630_green-abstract-windows-8-1-wallpapers_2560x1600_h.jpg',
        'https://fgcphotos.com/wp-content/gallery/abstract/e-ear-close.jpg',
        'https://www.teamunify.com/css/pro/cust_stock_bg/abstract_green.jpg',
        'https://www.artsrevo.com/wp-content/uploads/2018/06/IMG_4324.jpg',
        'https://vignette.wikia.nocookie.net/survivor-org/images/3/3c/Abstract-vista-wallpaper-windows-desktop-background-1260x1680.jpg/revision/latest/scale-to-width-down/2000?cb=20141221024347'
      ],
      current: 0
    }
  },
  methods:{
    previous () {
      this.current = Math.abs((--this.current) % this.images.length)
    },
    next () {
      this.current = (++this.current) % this.images.length
    }
  },
  mounted () {
    setInterval(this.next, 3000)
  }
}
</script>

<style lang="sass" scoped>
.slideshow-container
  height: 100vh
  background: darkgreen
  color: white
  position: relative


.slideshow-container
  .content
    position: absolute
    left: 0
    right: 0
    top: 0
    bottom: 0
    margin: auto
    text-align: center
    height: 15rem  
    h1
      color: #EEE
      font-family: "Just Another Hand",cursive
      font-size: 4rem
      text-transform: uppercase
    p
      color: rgba(187, 180, 180, 0.7)
      font-size: 20px  
      margin-bottom: 10px
      a 
        color: rgba(187, 180, 180, 0.7)

    button 
      padding: 1rem 2rem
      border-radius: 30px
      background: white
      color: #b2d430
      border: 2px solid #AAA
      cursor: pointer
      margin: 1rem
     

.slideshow-container
  .slides
    list-style: none
    margin: 0
    padding: 0
    li
      position: absolute
      top: 0
      bottom: 0
      left: 0
      right: 0
      background-attachment: fixed
      background-size: cover
      visibility: hidden
      &.active
        visibility: visible

.slideshow-container
  .navigators
    position: absolute
    display: flex
    justify-content: space-between
    height: 5rem
    margin: auto 
    top: 0
    bottom: 0
    left: 0
    right: 0
    z-index: 5
    padding: 0 2rem
    .prev, .next
      padding: 20px
      border-radius: 3rem 
      background: none
      color: white
      font-size: 2.5rem
      cursor: pointer
 
</style>


