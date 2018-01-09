<template>
  <div id="app">
    <pre-input></pre-input>
  </div>
</template>

<script>
//Valinput means the text inputs that will be used to validate the new account and the passwords strengths
import InputPreValidation from './components/InputPreValidation'
export default {
  name: 'app',
  components: {
   'pre-input' : InputPreValidation
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
