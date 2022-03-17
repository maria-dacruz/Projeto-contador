<template>
  <div id="app">
    
    <ProjContador/>
  </div>
</template>

<script>
import ProjContador from './components/ProjContador.vue'

export default {
  name: 'App',
  components: {
    ProjContador,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
