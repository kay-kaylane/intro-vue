<!-- Crie um componente com três slots; header, default e footer -->
 <script setup>

</script>
<template>
    <div class="model">
        <header>
            <slot name="header">Cabeçalho Padrão</slot>
        </header>
        <main>
            <slot name="default">Conteúdo Padrão</slot>
        </main>
        <footer>
            <slot name="footer">Rodapé Padrão</slot>
        </footer>
    </div>
</template>