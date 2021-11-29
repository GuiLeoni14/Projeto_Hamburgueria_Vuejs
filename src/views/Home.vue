<template>
    <section class="s-home">
        <Banner/>
        <div class="container">
            <h1>Monte o seu Burguer: </h1>
        </div>
    </section>
</template>

<script>
import Banner from '../components/Banner.vue'
// @ is an alias to /src
export default {
    name: 'Home',
    components: {
        Banner,
    }
}
</script>

<style lang="scss" scoped>
    .s-home{
        padding-top: 15rem;
    }
</style>