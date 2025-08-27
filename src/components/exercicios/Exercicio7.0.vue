<script setup>
import { ref } from 'vue'

const estado = ref('inativo')

function avancarEstado(){
    if (estado.value === 'inativo'){
        estado.value = 'carregando'
        setTimeout(() => {
            estado.value = 'ativo'
        }, 2000)
    } else if (estado.value === 'ativo'){
        estado.value = 'inativo'
    }
}
</script>

<template>
  <div>
    <button
      :class="{
        ativo: estado === 'ativo',
        inativo: estado === 'inativo',
        carregando: estado === 'carregando'
      }"
      :disabled="estado === 'carregando'"
      @click="avancarEstado"
    >
      <span v-if="estado === 'ativo'">Ativo</span>
      <span v-else-if="estado === 'inativo'">Inativo</span>
      <span v-else>Carregando...</span>
    </button>
  </div>
</template>

<style scoped>
.ativo {
  color: green;
}
.inativo {
  color: red;
}
.carregando {
  color: blue;
}
</style>


