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
// import ButtonComponent from './components/exercicios/Exercicio11.vue'
import model from './components/exercicios/Exercicio12.vue'
// import { ref } from 'vue';
// import Exemplo11Emits from './components/Exemplo11Emits.vue';
 import Card from './components/exercicios/Exercicio13.vue';

</script>

<template>

   <!-- <Exemplo11Emits @update="atualizarTotal"></Exemplo11Emits>
   <p>Total de cliques: {{ totalCliques }}</p> -->
   <!-- <ButtonComponent>Clique aqui</ButtonComponent> -->
    <!-- <model>
        <template #header>
            <h2>Header Customizado.</h2>
        </template>
        <p>Conteúdo do modelo personalizado via slot padrão.</p>
        <template #footer>
            <p>Footer Customizado.</p>
        </template>
    </model> -->
    <Card titulo="Meu Título" descricao="Minha Descrição">
     <template #header>
          <h2>Header Customizado</h2>
     </template>
     <p>Conteúdo do card personalizado via slot padrão.</p>
     <template #footer>
          <p>Footer Customizado</p>
     </template>
    </Card>
        
</template>