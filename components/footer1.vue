<template lang="pug">
.Footer
    .content
        .about
            h3 ABOUT OUR FARM
            p Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.
            a(href="#") Readmore..
        .links
            h3 QUICK LINKS
            ul
                li
                    a(href="#") Organic Fruits
                li
                    a(href="#") Organic Vegitables
                li
                    a(href="#") Non-GMO Products
                li
                    a(href="#") Locally Grown Products
        
        .product
            h3 PRODUCTS
            ul
                li
                    a(href="#") Organic Fruits
                li
                    a(href="#") Organic Vegitables
                li
                    a(href="#") Non-GMO Products
                li
                    a(href="#") Locally Grown Products

        .subscribe
            h3 SUBSCRIBE
            p Far far away behind the word mountains far from.
            input(type="text" placeholder="Enter your mail..")

</template>
<script>

export default {
    
}
</script>
<style lang="sass" scoped>
$color: #FFF
$green: #B2D430
.Footer
   
    padding: 5%
    height:  50%
    background: url("https://uicookies.com/demo/theme/green/img/slider_2.jpg") no-repeat
    background-attachment: fixed
    background-size: cover
    .content  
        justify-content: space-evenly
        margin-left: auto
        margin-right: auto 
        max-width: 1000px
        width: 100%
        @media (min-width: 800px)
            display: flex
            align-items: flex-start
        .about, .links, .product, .subscribe
            flex: 1
            padding: 1rem

.Footer
    .content
        .about  
            margin-bottom: 2rem
            h3
                text-transform: uppercase
                font-size: 14px
                letter-spacing: .2em
                margin-bottom: 30px
                color: $color
            p
                margin-bottom: 1rem
                color: $color
            a
                text-decoration: none
                color: $green


        .links
            margin-bottom: 2rem
            h3
                text-transform: uppercase
                font-size: 14px
                letter-spacing: .2em
                margin-bottom: 30px
                color: $color
            ul
                
                padding: 0
                li
                    list-style: none
                    
                    a
                        text-decoration: none
                        color: $green
        .product
            margin-bottom: 2rem
            h3
                text-transform: uppercase
                font-size: 14px
                letter-spacing: .2em
                margin-bottom: 30px
                color: $color
            ul
                padding: 0
                li
                    list-style: none
                    a
                        text-decoration: none
                        color: $green
        .subscribe
            margin-bottom: 2rem
            h3  
                text-transform: uppercase
                font-size: 14px
                letter-spacing: .2em
                margin-bottom: 30px
                color: $color
            p 
                color: $color
                margin-bottom: 0.5rem
</style>
