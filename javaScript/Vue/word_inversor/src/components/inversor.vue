<template>
    <div class="main">
        <div>
            <input id="textEnt" v-model="message" type="text" placeholder="Digite aqui o texto a ser revertido...">
        </div>

        <div>
            <h1 id="reversed">{{ reversed }}</h1>
        </div>
    </div>
  
</template>

<script>
    export default {
        name: 'inversor',
        data(){
            return{
                message: ''
            }            
        },
        computed: {
            reversed: function () {
                return this.message.split('').reverse().join('')
            }
        }
    }
</script>

<style scoped>

    .main{
        width: 50%;
        height: 50%;
        margin: 0 auto;
        padding: 20px;
        border-top: 1px solid #ccc;
        border-left: 1px solid #ccc;
        border-bottom: 1px solid #999;
        border-right: 1px solid #999;
        box-shadow: 0 1px 1px #cccccc;
        border-radius: 10px;
    }

    #textEnt{
        width: 50%;
        border-radius: 10px;
        height: 50px;
    }
</style>
