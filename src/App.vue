<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <j-browse :assembly="assembly" :tracks="tracks"/>
  </div>
</template>

<script>
import assembly from '../src/assembly'
import tracks from '../src/tracks'
import JBrowse from './components/JBrowse.vue'
export default {
  name: 'App',
  data(){
    return {
      assembly:assembly,
      tracks:tracks
    }
  },
  components: {
    JBrowse
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
