<template>
  <div id="app">
    <Header></Header>
    <bd></bd>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import bd from './components/tbody.vue'

export default {
  name: 'App',
  components: {
    Header,
    bd
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  width: 100%;
  height: 100%;
  position: absolute;
  background-color: black;
}

</style>
