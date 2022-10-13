<template>
  <h1 ref="greet">hi {{ title }}</h1>
  <input type="text" ref="name">
  <button @click="clickHandler">Click</button>
</template>

<script>
export default {
  data(){
    return{
      title:'U dont know me'
    }
  },
  methods:{
    clickHandler()
    {
      this.$refs.name.focus()
      this.$refs.greet.textContent = 'hi there'
    }
  }
}
</script>

<style>
h1{
  color:blue;
}
</style>