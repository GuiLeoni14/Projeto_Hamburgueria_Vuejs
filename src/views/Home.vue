<template>
    <section class="s-home">
        <Banner/>
        <div class="container">
            <div class="main_home">
                <h1>Monte o seu Burguer: </h1>
                <BurguerForm/>
            </div>
        </div>
    </section>
</template>

<script>
import Banner from '../components/Banner.vue'
import BurguerForm from '../components/BurguerForm.vue'
// @ is an alias to /src
export default {
    name: 'Home',
    components: {
        Banner,
        BurguerForm,
    }
}
</script>

<style lang="scss" scoped>
    .s-home{
        padding-top: 15rem;
        .container{
            .main_home{
                padding: 8rem 0rem 10rem 0rem;
                h1{
                    text-align: center;
                }
            }
        }
    }
</style>