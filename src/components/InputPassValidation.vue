<template>
  <div>
      <div>
          <passw-input :inputType="pass" @checkData="checkPassword"></passw-input>
          <ul>
              <li>Pelo menos 6 caracteres</li>
              <li>Pelo menos 1 letra maiúscula</li>
              <li>Pelo menos 1 número</li>
          </ul>
          <passw-input :inputType="passconf"></passw-input>
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
                inputVal: '',
                color: 'grey',
                pass: {typo: "password", label: "Senha", id: "password"},
                passconf: {typo: "password", label: "Confirmar Senha", id: "password-confirmation"}
            }
        },
        computed:{
            checkPassword: function(sizeInp){
               return this.inputVal = sizeInp
            }
        },
        watch:{
            checkSixMin: function(val){
                console.log(val)
            }
        }
    
    }
</script>

<style scoped>
    ul li{
        text-align: left;
        
    }
    span{
        color: #010101;
    }

    ul.valid{
        color: red;
    }
</style>
