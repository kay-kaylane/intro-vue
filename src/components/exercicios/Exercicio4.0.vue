<script setup>
let texto = '<strong> Texto </strong>'
</script>

<template>
    <div v-html="texto"></div>
    <div>{{ texto }}</div>
</template>