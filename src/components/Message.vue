<template>
    <div class="message_container">
        <p>{{ msg }}</p>
    </div>
</template>
<script>
export default {
    name: 'Message',
    props: {
        msg:  String
    }
}
</script>
<style lang="scss" scoped>
    .message_container{
        color: #004085;
        background-color: #cce5ff;
        border: 2px solid #b8baff;
        border-radius: 0.5rem;
        padding: 1rem;
        width: 100%;
        max-width: 40rem;
        margin: 3rem auto;
        P{
            text-align: center;
            font-size: 2rem;
        }
    }
</style>