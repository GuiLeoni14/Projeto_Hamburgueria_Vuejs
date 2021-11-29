<template>
    <div class="main_form">
        <p>Component de mensagem</p>
        <div class="form">
            <form action="">
                <div class="input_container">
                    <label for="nome">Nome do cliente: </label>
                    <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite o seu nome: ">
                </div>
                <div class="input_container">
                    <label for="pao">Escolha o pão: </label>
                    <select name="pao" id="pao" v-model="pao">
                        <option value="">Selecione o seu pão: </option>
                        <option value="integral">Integral</option>
                    </select>
                </div>
                <div class="input_container">
                    <label for="carne">Escolha a carne: </label>
                    <select name="carne" id="pao" v-model="carne">
                        <option value="">Selecione o tipo de carne: </option>
                        <option value="maminha">Maminha</option>
                    </select>
                </div>
                <div class="input_container opcionais_container">
                    <label id="opc_title" for="opcionais">Selecione os opcionais: </label>
                    <div class="checkbox_container">
                        <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                        <span>Salame</span>
                    </div>
                    <div class="checkbox_container">
                        <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                        <span>Salame</span>
                    </div>
                </div>
                <div class="input_container">
                    <input type="submit" class="submit_btn" value="Criar seu Burguer!">
                </div>
            </form>
        </div>
    </div>
</template>
<script>
export default {
    name: 'BurguerForm',
}
</script>
<style lang="scss" scoped>
    .main_form{
        margin-top: 10rem;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        width: 100%;
        .form{
            width: 100%;
            max-width: 40rem;
            form{
                .input_container{
                    display: flex;
                    flex-direction: column;
                    margin-bottom: 2rem;
                    label{
                        font-size: 2rem;
                        font-weight: bold;
                        margin-bottom: 1.5rem;
                        color: #222;
                        padding: 0.5rem 1rem;
                        border-left: 0.4rem solid #fcba03;
                    }
                    input, select{
                        font-size: 1.5rem;
                        padding: 0.5rem 1rem;
                        width: 30rem;
                    }
                    option{
                        font-size: 1.5rem;
                    }
                    select{
                        border: 1px solid #222;
                        border-radius: 0.2rem;
                    }
                    .submit_btn{
                        background-color: #222;
                        color: #fcba03;
                        font-weight: bold;
                        border: 0.2rem solid #222;
                        padding: 1rem;
                        font-size: 1.6rem;
                        margin: 0 auto;
                        cursor: pointer;
                        border-radius: 0.5rem;
                        transition: all .5s;
                        &:hover{
                            background-color: transparent;
                            color: #222;
                        }
                    }
                }
                .opcionais_container{
                    flex-direction: row;
                    flex-wrap: wrap;
                    #opc_title{
                        width: 100%;
                    }
                    .checkbox_container{
                        display: flex;
                        align-items: center;
                        width: 50%;
                        margin-bottom: 2rem;
                        span, input{
                            width: auto;
                        }
                        input{
                            cursor: pointer;
                        }
                        span{
                            font-size: 1.5rem;
                            font-weight: bold;
                            margin-left: 0.6rem;
                        }
                    }
                }
            }
        }
    }
</style>