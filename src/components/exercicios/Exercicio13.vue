<!-- Cards com Props + Named Slots -->

<script setup>
    const props = defineProps({
        titulo: String,
        descricao: String,
    })
</script>

<template>
    <div class="Card">
        <header>
            <h1>{{ titulo }}</h1>
            <h2>{{ descricao }}</h2>
        </header>
        <main>
            <slot>Conteúdo Padrão</slot>
        </main>
        <footer>
            <slot name="footer">Rodapé Padrão</slot>
        </footer>
    </div>
</template>


 