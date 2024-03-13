<script setup>
import { ref } from 'vue'
  import Perguntas from './components/Perguntas.vue';

  var count = ref(0)

  const perguntas = [
    {
      titulo : "Titulo 1",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 2
    },
    {
      titulo : "Titulo 2",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 2
    },
    {
      titulo : "Titulo 3",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 2
    },
    {
      titulo : "Titulo 4",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 2
    },
  ]

</script>

<template>
  <div class="container">

    <div v-for="(pergunta, index) in perguntas" >
      <Perguntas v-if="count == index"
      :title="pergunta.titulo"
      :resposta1="pergunta.resposta1"
      :resposta2="pergunta.resposta2"
      :resposta3="pergunta.resposta3"
      :resposta4="pergunta.resposta4"
      :correta="pergunta.correta"
      />
    </div>

    
    <div  class="container text-center">
    <div class="row align-items-center">
      <div class="col">
        <p><button @click="count--" type="button" class="btn btn-outline-secondary">Voltar</button></p>
      </div>
      <div class="col">
        <p><button @click="count++" type="button" class="btn btn-outline-secondary">Próximo</button></p>
      </div>
    </div>
  </div>
  </div>


</template>
<style>
</style>

<style scoped>
</style>
