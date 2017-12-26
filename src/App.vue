<template>
  <div id="app">
    <img src="./assets/logo.png">
    <InitiativeForm/>
  </div>
</template>

<script>
import InitiativeForm from './components/InitiativeForm'

export default {
  name: 'app',
  components: {
    InitiativeForm
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
