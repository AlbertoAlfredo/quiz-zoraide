<script setup>
import { ref } from 'vue'
  import Perguntas from './components/Perguntas.vue';
  import Image01 from './assets/01.png'
  import Image02 from './assets/02.png'

  var count = ref(0)

  const perguntas = [
    {
      titulo : "Entretanto no ábaco da figura, os adesivos não seguiram a disposição usual. <br /><img src='"+Image01+"' /> <br /> Nessa disposição, o número que está representado na figura é:",
      resposta1: "A) 46 171",
      resposta2: "B) 147 016",
      resposta3: "C) 171 064",
      resposta4: "D) 460 171",
      correta: 2
    },
    {
      titulo : "Realizando a decomposição de um número, encontramos a soma 50000 + 300 + 20 + 1. O número decomposto foi:",
      resposta1: "A) 53210",
      resposta2: "B) 53021",
      resposta3: "C) 50321",
      resposta4: "d) 500321",
      correta: 3
    },
    {
      titulo : "No número 153902, o valor posicional do algarismo 9 é:",
      resposta1: "A) 9",
      resposta2: "B) 90",
      resposta3: "C) 900",
      resposta4: "D) 9000",
      correta: 3
    },
    {
      titulo : "Nos números 1320, 203 e 2932, o valor posicional do algarismo 3 é, respectivamente:",
      resposta1: "A) centena, dezena e unidade",
      resposta2: "B) unidade, dezena e centena",
      resposta3: "C) dezena, unidade e centena",
      resposta4: "D) centena, unidade e dezena",
      correta: 4
    },
    {
      titulo : "Em um trabalho da escola, Márcio e Tiago estavam no mesmo grupo, então Márcio anotou o telefone de Tiago em um papel de anotações. Porém, por descuido de Márcio, durante o lanche, ele derramou katchup em um dos dígitos conforme a imagem a seguir: <br /><img src='"+Image02+"' /> <br /> O número que está manchado corresponde à:",
      resposta1: "A) unidade",
      resposta2: "B) dezena",
      resposta3: "C) centena",
      resposta4: "D) dezena de milhar",
      correta: 4
    },
    {
      titulo : "Na campanha de vacinação de uma cidade, foram vacinadas 380.210 crianças. O nome desse número por extenso é:",
      resposta1: "A) trezentos e oitenta mil e duzentos e dez",
      resposta2: "B) trinta e oito mil e duzentos e dez",
      resposta3: "C) trezentos e oitenta e dois mil e cem",
      resposta4: "D) trezentos milhões duzentos e dez mil",
      correta: 1
    },
    {
      titulo : "Sobre o número 123.456.789.201, podemos afirmar que:",
      resposta1: "A) 789 pertence à classe das unidades simples",
      resposta2: "B) 123 pertence à classe das dezenas",
      resposta3: "C) 456 pertence à classe dos milhões",
      resposta4: "D) 201 pertence à classe dos milhares",
      correta: 3
    },
    {
      titulo : "Um padeiro produziu 1423 pães durante a semana. Esse número é formado por:",
      resposta1: "A) 1 unidade de milhar, 4 centenas, 2 dezenas e 3 unidades",
      resposta2: "B) 1 unidade de milhão, 4 unidades de milhar, 2 dezenas e 3 unidades",
      resposta3: "C) 1 centena, 4 dezenas e 2 unidades",
      resposta4: "D) 1 unidade de milhar, 4 centenas, 3 dezenas e 2 unidades",
      correta: 1
    },
    {
      titulo : "Dentre os números 2.501, 4.235, 1.536, 4.057, 30.597 e 41.500, quantos têm o algarismo 5 ocupando a ordem das centenas?",
      resposta1: "A) 1",
      resposta2: "B) 2",
      resposta3: "C) 3",
      resposta4: "D) 4",
      correta: 4
    },
    {
      titulo : "A quantidade de números com três algarismos diferentes que podemos formar com os números 1,4 e 5 usando os três algarismos são:",
      resposta1: "A) 2",
      resposta2: "B) 3",
      resposta3: "C) 4",
      resposta4: "D) 6",
      correta: 4
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
    },
    {
      titulo : "Titulo 6",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      correta: 1
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
