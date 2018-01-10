<template>
  <div>
      <div>
          <passw-input :inputType="pass"></passw-input>
      </div>
  </div>
</template>

<script>

    import inputDefault from "./general-use/inputDefault";
    export default {

        name: 'PassValidation',
        components: {
            'passw-input' : inputDefault
        },

        data(){
            return{
                pass: {typo: "password", label: "Senha", id: "password"},
                passconf: {typo: "password", label: "Senha", id: "password-confirmation"}
            }
        }
    
    }
</script>

<style>

</style>
