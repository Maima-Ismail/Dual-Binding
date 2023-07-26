<template>
  <twoWay />
</template>

<script>
import twoWay from './components/twoWay.vue'

export default {
  name: 'App',
  components: {
    twoWay,
  },
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
