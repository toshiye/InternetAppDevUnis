<template>
  <div id="app">
    <Inversor/>
  </div>
</template>

<script>
import Inversor from './components/inversor'

export default {
  name: 'App',
  components: {
    Inversor
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
