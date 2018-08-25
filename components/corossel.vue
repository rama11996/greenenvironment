<template lang="pug">
.slider-corosel
  .organic
    h3 100% Organic
  .subtitle
    p A new website template by 
      a(href='https://uicookies.com/') uicookies.com
      p under lisence
      a(href='https://uicookies.com/license/') Creative Commons3.0  
  .button
    button(type="submit") Get This 

</template>
<style lang="sass" scoped>
.slider-corosel
  background: #e9e9e5  
  margin: 2px 2px
  .organic
    color: white
    text-align: center
    font-size: 60px
    font-family: Courier New
  .subtitle
    color: rgba(187, 180, 180, 0.7)
    text-align: center
    font-size: 20px  
    p
    margin-bottom: 20px
    a
      text-decoration: underline 
      color: rgba(187, 180, 180, 0.7) 
  .button
    button
      border: 2px solid #fff
      background: white
      padding: 15px 60px
      border-radius: 30px
      color: #b2d430
      align-items: center
      margin-left: 43%
@media ( max-width: 550px )  
  .slider-corosel
    .button
      button    
        margin-left: 25%
    </style>

