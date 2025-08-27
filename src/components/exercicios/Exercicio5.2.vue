<script setup>
    import {ref} from 'vue'
    let peso = ref('')
    let altura = ref('')
   
    
    function IMC (peso, altura){
    return peso / (altura * altura)
}

   
</script>

<template>
    <p>Digite seu peso: {{ peso }}</p>
    <input type="number" v-model="peso"></input>

    <p>Digite sua altura: {{ altura }}</p>
    <input type="number" v-model="altura"></input>

    <p>Seu IMC é: {{ IMC(peso,altura) }}</p>

</template>

