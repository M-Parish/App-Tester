<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div>
      <label>Zip Code</label>
      <input v-model="zipCode">
    </div>
    <button @click="searchForWeather()">Search</button>
    <div>
      {{zipCode}}
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data() {
    return {
      zipCode: ''
    }
  },
  components: {
    HelloWorld
  },
  methods: {
    searchForWeather() {
      console.log('do the thing');
    }
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
