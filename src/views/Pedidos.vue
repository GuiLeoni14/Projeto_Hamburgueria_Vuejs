<template>
    <section class="s-pedidos">
        <div class="container">
            <h1>Gerenciar Pedidos:</h1>
            <Dashboard/>
        </div>
    </section>
</template>
<script>
import Dashboard from '../components/Dashboard.vue'
export default {
    name: 'Pedidos',
    components: {
        Dashboard,
    }
}
</script>

<style lang="scss" scoped>
    .s-pedidos{
        padding-top: 15rem;
    }
</style>