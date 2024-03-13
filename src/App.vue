<script setup>
  import Perguntas from './components/Perguntas.vue';

  const perguntas = [
    {
      titulo : "Titulo 1",
      resposta1: "Resposta 01",
      resposta2: "Resposta 02",
      resposta3: "Resposta 03",
      resposta4: "Resposta 04",
      teste: 2
    }
  ]

</script>

<template>
  <div class="container">

    <Perguntas 
      title="Teste"
      resposta1="resposta 1"
      resposta2="resposta 2"
      resposta3="resposta 3"
      resposta4="resposta 4"
      correta = 1
    />
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
