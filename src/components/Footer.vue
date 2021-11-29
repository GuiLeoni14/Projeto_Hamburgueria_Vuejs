<template>
    <footer id="footer">
        <p>Make Your Burguer &copy; 2021</p>
    </footer>
</template>
<script>
export default {
    name: 'Footer',
}
</script>

<style lang="scss" scoped>
    footer{
        padding: 10rem;
        border-top: 0.4rem solid #111;
        background-color: #222;
        width: 100%;
        color: #fcba03;
        p{
            font-size: 2rem;
            text-align: center;
        }
    }
</style>