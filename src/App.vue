<script setup>
import { livros } from '@/_data/livros'
//exportando do livro.js E importanto para o app
</script>

<template>
  <h1>Minha Livraria</h1>
  <div class="livros">
    <div class="card-livro" v-for="livro in livros" :key="livro.id">
        <img :src="livro.cover" class="livro-cover" >
      <p class="livro-title">{{ livro.title }}</p>
      <p class="livro-author">{{ livro.author }}</p>
      <p class="livro-price">{{ livro.price }}</p>  
    </div>
  </div>
</template>

<style scoped>

</style>