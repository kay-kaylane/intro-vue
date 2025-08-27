<script setup>
// import Exemplo01 from './components/Exemplo01Interpolacao.vue'
// import Exemplo3 from './components/Exemplo03For.vue'
// import Exemplo06 from './components/Exemplo06Classe.vue'
//import Exercicio52 from './components/exercicios/Exercicio5.2.vue'
// import Exercicio6 from './components/exercicios/Exercicio6.0.vue'
// import Exemplo7 from './components/Exemplo07Clique.vue'
// import Exercicio7 from './components/exercicios/Exercicio7.0.vue'
// import Exemplo9 from './components/Exemplo09Enviar.vue'
import UserCard from './components/Exemplo10Props.vue';
import UserCard from './components/Exercicio9.0.vue';
</script>

<template>
    <Exemplo9></Exemplo9>
    <UserCard nome="Kaylane" idade="17" telefone="12343211" :ativo="True"></UserCard>
    <ProductCard title="Smartphone" price="1999.99"  image="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR72Hz7MdPnzJyIoEiALo0PSP6DPUL01Ztzgw&s" :in-stock="True"></ProductCard>
</template>