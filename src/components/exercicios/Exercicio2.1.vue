<script setup>
    let usuarioLogado = false // Se colocar false, o h1 não será exibido
</script>

<template>
    <h1 v-if="usuarioLogado">Bem-vindo!</h1>
    <p v-else><button>Faça login</button></p>
</template>