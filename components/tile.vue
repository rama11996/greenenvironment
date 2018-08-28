<template lang="pug">
.organic-card
    .tilecard
        .card(v-for="n in 6")
            .image
                img(src="https://uicookies.com/demo/theme/green/img/img_1.jpg")
            .content
                .name
                    h3 Organic Dragon Fruite
                .description
                    p Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.
                .button
                    button(type="submit") view details
</template>
<script>
export default {
    
}
</script>
<style lang="sass" scoped>
$green: #B2D430
.organic-card
    padding: 2%
    display: flex
    flex-wrap: wrap
    justify-content: center
    background: #EEE
    .tilecard
        display: flex
        flex-wrap: wrap
        justify-content: center
        margin-left: auto
        margin-right: auto 
        width: 1100px
        .card
            border-radius: 0.5rem
            width: 300px 
            background: #FFF
            margin: 2%
            @media(max-width: 700px)
                width: 550px
            .image
                img
                    width: 100%
                    border-radius: .5rem
            .content   
                align-items: center
                .name
                    margin: 1rem
                    opacity: 0.6
                .description
                    p 
                        margin: 1rem
                        margin-bottom: 1.5rem
                        font-size: 16px
                        font-weight: 300
                        line-height: 1.7
                        color: #7e8890
                .button
                    margin: 5%
                    button
                        background: $green
                        border-radius: 20px
                        color: #fff
                        padding: 0.7rem
                        


</style>
