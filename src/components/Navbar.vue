<template>
    <div id="nav">
        <div class="container">
            <router-link to="/" class="img_logo">
            <img :src="logo" :alt="alt" id="logo">
            </router-link>
            <nav>
                <ul>
                    <li><router-link to="/">Home</router-link></li>
                    <li><router-link to="/pedidos">Pedidos</router-link></li>
                </ul>
            </nav>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Navbar',
    props: ['logo', 'alt']
}
</script>
<style lang="scss" scoped>
    #nav{
        background-color: #222;
        border-bottom: 0.4rem solid #111;
        position: fixed;
        width: 100%;
        height: 15rem;
        display: flex;
        align-content: center;
        justify-content: center;
        .container{
            display: flex;
            align-items: center;
            justify-content: space-between;
            .img_logo{
                img{
                    width: 10rem;
                    height: 10rem;
                }
            }
            nav{
                ul{
                    display: flex;
                    align-items: center;
                    justify-content: space-between;
                    li{
                        font-size: 2rem;
                        &:not(:first-child){
                            margin-left: 8rem;
                        }
                        a{
                            color: #fcba03;
                            transition: all .3s;
                            &:hover{
                                color: #fff;
                            }
                        }
                    }
                }
            }
        }
    }
</style>