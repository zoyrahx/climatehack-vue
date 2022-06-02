<template>
  <div id="app">
    <ClimateHack msg="Climate Hackathon 2022"/>
  </div>
</template>

<script>
import ClimateHack from './components/ClimateHack.vue'

export default {
  name: 'App',
  components: {
    ClimateHack
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
