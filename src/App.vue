<template>
  <Navbar />
</template>

<script>
import Navbar from './components/Navbar.vue';


export default{
  name: 'App',
  components:{
    Navbar,
  }
}
</script>

<style lang="scss">
@import './global.scss';
</style>
