<template>
  <div id="app">
    <img src="./assets/logo.png">
    <div id="coonsContainer">
      <CoonsList/>

    </div>
  </div>
</template>

<script>
import CoonsList from './components/CoonsList'

export default {
  name: 'app',
  components: {
    CoonsList
  }
}
</script>

<style>
#coonsContainer {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
