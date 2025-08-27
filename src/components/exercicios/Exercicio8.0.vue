<script setup>
import { ref } from 'vue'
let inputValue = ref('')

function mensagem(){
    alert(`Executando a função: ${inputValue.value}`)
}
</script>

<template>
<input type="text" @keydown.enter="mensagem" v-model="inputValue"></input>
</template>