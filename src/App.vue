<script setup>
import { ref } from 'vue'
  import Perguntas from './components/Perguntas.vue';
  import Image01 from './assets/01.png'

  var count = ref(0)

  const perguntas = [
    {
      titulo : "Entretanto no ábaco da figura, os adesivos não seguiram a disposição usual. <br /><img src='"+Image01+"' /> <br /> Nessa disposição, o número que está representado na figura é:",
      resposta1: "A) 46 171",
      resposta2: "B) 147 016",
      resposta3: "C) 171 064.",
      resposta4: "D) 460 171.",
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
    {
      titulo : "Titulo 5",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 3
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
  ]

</script>

<template>
  <div style="width: 70rem;">
  

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
        <p><button v-if="count > 0" @click="count--" type="button" class="btn btn-outline-secondary">Voltar</button></p>
      </div>
      <div class="col">
        <p><button v-if="count < perguntas.length" @click="count++" type="button" class="btn btn-outline-secondary">Próximo</button></p>
      </div>
    </div>
  </div>
  </div>


</template>
<style>
</style>

<style scoped>
</style>
