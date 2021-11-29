<template>
    <Navbar :logo="logo_src" :alt="app_name" />
    <router-view/>
    <Footer/>
</template>
<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
export default {
    components: {
        Navbar,
        Footer,
    },
    data(){
        return{
            logo_src: '/img/logo.png',
            app_name: 'Make your burguer'
        }
    }
}
</script>
<style lang="scss">
    *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    border: none;
    outline: none;
    list-style: none;
    text-decoration: none;
    font-family: 'Inter', sans-serif;
    }
    html{
        font-size: 62.5%;
    }

    .container{
    width: 100%;
    max-width: 121.6rem;
    padding: 0 1.5rem;
    margin: 0 auto;
    }

    h1{
        color: #222;
        font-size: 4.2rem;
    }

    @mixin responsive($ScrennWidth) {
        @media(max-width: $ScrennWidth){
            @content;
        }
    }

    @mixin flex($direction, $align, $justify) {
        display: flex;
        flex-direction: $direction;
        align-items: $align;
        justify-content: $justify;
    }

</style>
