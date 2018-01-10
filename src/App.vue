<template>
  <div id="app">
    <login-card></login-card>
  </div>
</template>

<script>
import loginCard from './components/login-card.vue'
export default {
  name: 'app',
  components: {
    'login-card' : loginCard
  }
}
</script>

<style>
*{
  box-sizing: border-box;
}

body{
  background-color: #eee;
}
#app {
  font-family: 'Proxima Nova', Georgia, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  }
</style>
