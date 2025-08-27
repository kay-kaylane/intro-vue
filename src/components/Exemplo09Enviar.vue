<script setup>
function validaFormulario(){
    alert('Formulário enviado com sucesso!')
    event.preventDefault() // Previne o envio do formulário
}
</script>
<template>
    <form action="https://g1.globo.com" @submit="validaFormulario">
        <input type="submit" value="Enviar Formulário"></input>
    </form>
</template>