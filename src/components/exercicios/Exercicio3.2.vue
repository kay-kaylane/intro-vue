<script setup>
let produtos = {nome: 'pão', preço: 5, categoria: 'padaria'}
</script>

<template>
    <div v-for="produto in produtos"> 
            <h3>{{ produtos.nome }}</h3>
            <p> Preço: {{ produtos.preço }}</p>
            <p> Categoria: {{ produtos.categoria }}</p>
    </div>
</template>

<style scoped>
.card {
    border: 1px solid aqua
}

</style>