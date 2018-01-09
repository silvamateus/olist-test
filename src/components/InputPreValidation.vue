<template>
<div>
    <div v-for="value in inputData" :key="value.id">
        <input-default v-bind:inputType="value"></input-default>
    </div>
  </div>
</template>


<script>
import inputDefault from "./inputDefault";

export default {
  name: "InputPreValidation",
  components: {
    "input-default" : inputDefault
  },

  data() {
    //Here data returns the Values we'll use to validate the password in the future
    return {
      inputData: {
        nameInput: { typo: "text", label: "Nome Completo", id: "name" },
        emailInput: { typo: "text", label: "E-mail", id: "e-mail" },
        passInput: { typo: "password", label: "Senha", id: "password" }
      }
    }
  }
}
</script>
