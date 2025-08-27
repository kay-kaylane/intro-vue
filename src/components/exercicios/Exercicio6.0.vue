<script setup>
let ativo = false
let inativo = false
let carregando = true
</script>

<template>
    <button :class="{
        'ok' : ativo,
        'falha' : inativo,
        'carregando' : carregando
    }">Clique aqui</button>
</template>

<style scoped>
.ok{
    color: green
} 
.falha {
    color: red
}
.carregando {
    color: blue
}

</style>