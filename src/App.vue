<script setup>
// import Exemplo01 from './components/Exemplo01Interpolacao.vue'
// import Exemplo3 from './components/Exemplo03For.vue'
// import Exemplo06 from './components/Exemplo06Classe.vue'
//import Exercicio52 from './components/exercicios/Exercicio5.2.vue'
// import Exercicio6 from './components/exercicios/Exercicio6.0.vue'
// import Exemplo7 from './components/Exemplo07Clique.vue'
// import Exercicio7 from './components/exercicios/Exercicio7.0.vue'
// import Exemplo9 from './components/Exemplo09Enviar.vue'
//import UserCard from './components/Exemplo10Props.vue';
//import UserCard from './components/Exercicio9.0.vue';
import { ref } from 'vue';
import Exemplo11Emits from './components/Exemplo11Emits.vue';
const totalCliques = ref(0)

function atualizarTotal(valor){
    totalCliques.value = valor
}

</script>

<template>
   <Exemplo11Emits @update="atualizarTotal"></Exemplo11Emits>
   <p>Total de cliques: {{ totalCliques }}</p>
</template>