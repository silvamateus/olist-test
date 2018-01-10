
<template>
    <div id='login'>
        <logo></logo>
        <pre-input></pre-input>
        <pass-input></pass-input>
    </div>
</template>

<script>
import Logo from './general-use/logo.vue'
//import the text inputs that will be used to validate the new account and the passwords strengths
import InputPreValidation from './InputPreValidation'
import PassValidation from './InputPassValidation'
export default {
  name: 'app',
  components: {
      'logo' : Logo,
      'pre-input' : InputPreValidation,
      'pass-input' : PassValidation
  }
}
</script>


<style>
    #login{
        background-color: #fefefe;
        width: 28em;
        padding: 3em;
    }
</style>
