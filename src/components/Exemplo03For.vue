<script setup>
let nomes = ['Daniel', 'Celso', 'Marlon']
</script>

<template>
    <ul>
        <li v-for="(nome, index) in nomes"> {{ index + 1 }}. {{ nome }}</li>
    </ul>
</template>

<style scoped>

</style>