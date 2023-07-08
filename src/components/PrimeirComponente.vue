<template>
  <h1>Olá Vue</h1>
  <p>Meu nome é {{ nome }}</p>
  <p>Eu tenho: {{ idade }} anos</p>
</template>

<script>
export default {
  name: 'PrimeiroComponente',
  data(){
    return{
      nome: 'Ramon',
      idade: 35,
    }
  }
}
</script>
