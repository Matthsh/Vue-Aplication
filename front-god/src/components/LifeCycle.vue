<template>
    <h1>Meu nome é: {{ name }}</h1>    
</template>

<script>
import { createDOMCompilerError } from '@vue/compiler-dom';

    export default {
        name: 'LifeCycle',
        data(){
            return{
                name: "Ainda não sei"
            }
        },
        created(){
            setTimeout(() => {
                this.name = "Mattheus"
            }, 1000)
        },
        mounted(){
            setTimeout(() => {
                this.name = "Pedro"
            }, 2000)
        }
    }
</script>