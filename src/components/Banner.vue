<template>
    <div class="main_banner">
        <div class="container">
            <h1>Make Your Burguer</h1>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Banner'
}
</script>
<style lang="scss" scoped>
    .main_banner{
        background: url("/img/burger.jpg") no-repeat center center;
        background-size: cover;
        background-position: 0rem -25rem;
        height: 50rem;
        .container{
            display: flex;
            align-items: center;
            justify-content: flex-start;
            height: inherit;
            h1{
                color: #fff;
                font-size: 4.5rem;
                background-color: #222;
                border-radius: 0.5rem;
                padding: 2rem 4rem;
            }
        }
    }
</style>