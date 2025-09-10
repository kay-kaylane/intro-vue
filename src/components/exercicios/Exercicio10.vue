<script setup>
const props = defineProps({
        name: String,
        price: Number,
    })
</script>

<template>
    <div class="card" v-if="name">
        <h3>{{ nome }}</h3>
        <p v-if="email">Email: {{ email }}</p>
        <p v-if="telefone">Telefone: {{ telefone }}</p>
        <span v-if="idade">{{ idade }} anos</span>
        <div :class="ativo ? 'ativo' : 'inativo'">{{ ativo ? 'Ativo' : 'Inativo' }}</div>
    </div>
</template>