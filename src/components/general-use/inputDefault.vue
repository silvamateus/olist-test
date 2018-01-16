<template>
  <div class='input-card'>
    <label :for="inputType.id" >{{inputType.label}}</label>
    <input :type="inputType.typo" v-model="checkInput" class='input-default' :id="inputType.id" >
  </div>
</template>

<script>
export default {
  name: "inputDefault",
  props: {
    inputType: {
      type: Object,
      require: true
    }
  },
  data() {
    return {};
  },
  methods:{
    checkPass(){
      this.$emit('checkInput', 'contentCheck')
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.input-card{
  display: flex;
  flex-direction: column;
  align-items: flex-start; 
  padding-bottom: 1em;
}

.input-default {
  outline: none;
  text-align: center left;
  background-color: #fefefe;
  border: 1px solid #e1e1e1;
  width: 90%;
  padding-top: 0.5em;
  padding-bottom: 0.5em;
  flex-grow: 1;
}

.input-card > label{
  font-size: 12px;
  padding-bottom: 4px;
}
</style>
