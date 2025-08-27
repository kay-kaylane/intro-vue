<script setup>
let compras = ['Pão', 'Leite', 'Ovos', 'Frutas']
</script>

<template>
    <ul>
        <li v-for="(compras, index) in compras"> {{ index + 1 }}. {{ compras }}</li>
    </ul>
</template>

<style scoped>
ul {
    list-style-type: none;
}

</style>