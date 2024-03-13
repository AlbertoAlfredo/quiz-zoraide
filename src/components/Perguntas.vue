<script setup>
  import { ref } from 'vue'
  defineProps(['title', 'resposta1', 'resposta2', 'resposta3', 'resposta4', 'correta'])

  

  var resposta = ref(false)
</script>

<template>
<div class="container-fluid">
  <header class="container">
    <h1>Quiz Zoraide</h1>
  </header>
  <div class="container">
    
    

    <h2>{{ title }}</h2>
  <div v-if="!resposta" class="container text-center">
    <div class="row align-items-center">
      <div class="col">
        <p><button @click="resposta = true" type="button" class="btn btn-outline-secondary">{{ resposta1 }}</button></p>
        <p><button @click="resposta = true" type="button" class="btn btn-outline-secondary">{{ resposta2 }}</button></p>
      </div>
      <div class="col">
        <p><button @click="resposta = true" type="button" class="btn btn-outline-secondary">{{ resposta3 }}</button></p>
        <p><button @click="resposta = true" type="button" class="btn btn-outline-secondary">{{ resposta4 }}</button></p>
      </div>
    </div>
  </div>


  <div v-if="resposta"  class="container text-center">
    <div class="row align-items-center">
      <div class="col">
        <p><button type="button" class="btn" :class="{'btn-danger': correta!=1, 'btn-success': correta==1}">{{ resposta1 }}</button></p>
        <p><button type="button" class="btn" :class="{'btn-danger': correta!=2, 'btn-success': correta==2}">{{ resposta2 }}</button></p>

      </div>
      <div class="col">
        <p><button type="button" class="btn" :class="{'btn-danger': correta!=3, 'btn-success': correta==3}">{{ resposta3 }}</button></p>
        <p><button type="button" class="btn" :class="{'btn-danger': correta!=4, 'btn-success': correta==4}">{{ resposta4 }}</button></p>

      </div>
      
      
    </div>
  </div>

  </div>
</div>
</template>
<style>
</style>

<style scoped>
</style>
