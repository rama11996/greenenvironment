<template lang="pug">
  .tile
    .fruit-profile(v-for="n in 6")
      img(src="https://uicookies.com/demo/theme/green/img/img_1.jpg")
      .content
        .name
          h3 Organic Dragon Fruit
        .description
          p Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.
        .button
          button(type="submit") View Details  
</template>
<style lang="sass" scoped>

.tile
  background: grey
  display: flex
  flex-wrap: wrap
  justify-content: center
  .fruit-profile
    width: 320px 
    background: white 
    border-radius: 1rem 
    margin-top: 2rem
    margin-left: 2rem
    margin-bottom: 2rem
    @media (max-width: 720px)
      width: 650px
      margin-right: 2rem
    img 
      width:  100%
      border-radius: 1rem
    .content  
      padding: 10px
      .name
        padding: 7px
      .description
        background: white
        opacity: 0.7
      .button
        justify-content: center
        display: flex
        padding: 10px
        button
          border: none
          padding: 10px
          background: #B2D430
          color: white 
          border-radius: 1rem
          cursor: pointer 
</style>
