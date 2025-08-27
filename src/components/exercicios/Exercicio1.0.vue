<!-- Nome, idade e profissao -->

<script setup>
let nome = 'Maria'
let idade = 18
let profissao = 'delegada'
</script>

<template>
    <p>{{ `Meu nome é: ${nome}` }}</p>
    <p>{{ `Tenho ${idade} anos e sou ${profissao}` }}</p>
</template>