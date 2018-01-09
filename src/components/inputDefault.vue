<template>
  <div>
    <p>{{inputType.label}}</p>
    <input :type="inputType.typo" class="input-default" :id="inputType.id" >
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
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input-default {
  outline: none;
  text-align: center left;
  background-color: #fefefe;
}
</style>
