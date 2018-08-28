<template lang="pug">
.navigation
  .container
    .logo
      | Green
    .menu(:class="{open: open}")
      .mask(@click="toggle()")
      nav
        .menu-item(v-for="item in menuItem") {{ item }}
    .hamburger(@click="toggle()", :class="{open: open}")
      span =
</template>

<script>
export default {
  data () {
    return {
      menuItem: ['Home', 'About', 'Gallery', 'Contact'],
      open: false
    }
  },
  methods: {
    toggle () {
      this.open = !this.open
    }
  }
}
</script>

<style lang="sass" scoped>

$green: #B2D430
$header-height: 4rem


@mixin full-screen
  position: fixed
  right: 0
  top: 0
  bottom: 0
  left: 0

.navigation
  background: #FFF

  .container
    max-width: 1200px
    height: $header-height
    margin: 0 auto
    position: relative
    display: flex
    justify-content: space-between
    align-items: center

  .logo
    font-size: 1.5rem
    font-weight: bold
    text-transform: uppercase
    color: $green
    @media (max-width: 1200px)
      padding-left: 1rem

  .hamburger
    position: absolute
    right: 0
    font-size: 2rem
    font-weight: bold
    height: $header-height
    width: $header-height
    padding: 0.5rem 0 0 1rem
    cursor: pointer
    z-index: 2
    display: none
    @media (max-width: 600px)
      display: block
      &.open
        background: #000
        color: #FFF

  .menu
    @media (max-width: 600px)
      display: none
      &.open
        @include full-screen
        display: block
        .mask
          @include full-screen

  .menu 
    nav
      display: flex
      @media (max-width: 600px)
        @include full-screen
        left: auto
        flex-direction: column
        background: #000
        color: #FFF
        width: 15rem
        padding-top: 4rem

    nav .menu-item
      padding: 1rem
      transition: color 0.3s
      cursor: pointer
      &:hover
        color: $green
      @media (max-width: 600px)
        padding: 1rem 2rem

</style>