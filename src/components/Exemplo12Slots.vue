<script setup>

</script>
<template>
    <div class="model">
        <div class="model-content">
        <header>
            <slot name="header">Cabeçalho Padrão</slot>
        </header>
        <main>
            <slot>Conteúdo Padrão</slot>
        </main>
        <footer>
            <slot name="footer">Rodapé Padrão</slot>
        </footer>
    </div>
    </div>
</template>