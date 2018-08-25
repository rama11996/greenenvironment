<template lang="pug">
  .pageheader
    .companyname
      h3 Green.
    #menus.menuitems
      ul
        li.home HOME
        li.about ABOUT
        li.gallery GALLERY
        li.contact CONTACT
    .icons(v-on:click="menu()") 
      .icon1  
      .icon2
      .icon3

</template>
<script>
export default {
  methods:{
    menu: function(){
      var x= document.getElementById("menus")
      if(x.className === "menuitems"){
        x.className += "responsive"
      }
      else{
        x.className = "menuitems"
      }
    }
  }
}
</script>

<style lang="sass" scoped>
.pageheader
  display: flex
  padding: 3rem
  background: #bee8f9
  .companyname
    color: green
    font-weight: bold
    font-size: 20px
  .menuitems
    margin-left: auto
    ul
      display: flex
      list-style: none
      justify-content: space-between
      li
        margin-left: 20px
        border-bottom: 2px solid #b2d430
     
    
@media (max-width: 500px )      
  .pageheader
    .menuitems
      ul
        display: none  
    .icons
      display: flex
      flex-direction: column
      padding: 2px
      .icon1, .icon2, .icon3
        float: right  
        display: block
        margin-top: 1rem
        width: 25px
        height: 3px
        background-color: white
        margin: 2px 0  
@media (max-width: 500px )
  .pageheader
    .icons
      position: absolute
      top: 3rem
      right: 2rem       
    .menuitemsresponsive
      ul
        list-style-type: none  
        position: absolute
        top: 3rem
        right: 0rem 
        width: 190px
        height: 50%
        background: black
        color: white
        li
          padding: 4px
          &hover
            background: red
</style>

