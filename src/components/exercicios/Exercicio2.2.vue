<script setup>
    let idade = 45
</script>

<template>
    <p v-if="idade <= 12">Criança</p>
    <p v-else-if= "idade <= 17">Adolescente</p>
    <p v-else-if= "idade <= 59">Adulto</p>
    <p v-else>Idoso</p>
</template>