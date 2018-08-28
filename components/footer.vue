<template lang="pug">
  .footer
    .contents
      .about
        h5 ABOUT OUR FARM
        p Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.
        a(href="#") Read More..
      .quicklinks
        h5 QUICK LINKS  
        ul
          li 
            a(href="#") Organic Fruits
          li 
            a(href="#") Organic Vegetables
          li 
            a(href="#") Non GMO Products
          li 
            a(href="#") Locally Grown Products
      .products    
        h5 Products
        ul
          li 
            a(href="#") Organic Fruits
          li 
            a(href="#") Organic Vegetables
          li 
            a(href="#") Non GMO Products
          li 
            a(href="#") Locally Grown Products
      .subscribe
        h5 Subscribe  
        p  Far far away, behind the word mountains
        input(type="text" placeholder="Enter your mail...")
        img(src="../assets/Images/submit.png")
    .copyrights
      .content 
       p © 2017 
        a(href="#") uiCookies:Green. 
        p Designed by
        a(href="#") uicookies.com 
      .social-networks
        ul
          li  
            img(src="../assets/Images/fb.png")
          li  
            img(src="../assets/Images/instagram.png")
          li  
            img(src="../assets/Images/twitter.png")     
</template>
<style lang="sass" scoped>
$green: #B2D430
$white: #fff
.footer 
  background: url("https://uicookies.com/demo/theme/green/img/slider_3.jpg")
  .contents 
    @media (min-width: 950px)
      display: flex
      justify-content: space-between
    .about
      margin-left: 2.5rem
      margin-top: 3rem
      color: $white
      h5
        padding-bottom: 20px
      p
        font-size: 15px  
      a
        color: $green 
      @media (min-width: 950px)
        width: 300px   
    .quicklinks
      h5
        margin-left: 2.5rem
        padding-bottom: 20px
        margin-top: 3rem
        color: $white
      ul
        li
          list-style: none
          a
            text-decoration: none
            color: $green       
    .products
      h5
        margin-left: 2.5rem
        padding-bottom: 20px
        margin-top: 3rem
        color: $white
      ul
        li
          list-style: none
          a
            text-decoration: none
            color: $green
            padding: 2px     
    .subscribe  
      margin-top: 3rem
      color: $white
      margin-left: 2.5rem
      p
        font-size: 15px
      h5
        padding-bottom: 20px
      input
        padding: 8px 
        border: none
        background: transparent
        border: 1px solid $white
      img
        padding: 8px  
      @media (min-width: 950px)
        width: 300px     
  .copyrights
    @media (min-width: 950px)
      display: flex
      justify-content: space-between
    padding: 2rem
    .content
      p
        color: $white
    .social-networks
      ul
        display: flex
        li
          padding: 20px
          list-style: none
          img
            background-color: $green 
            border-radius: 1rem
            height: 35px             
</style>

