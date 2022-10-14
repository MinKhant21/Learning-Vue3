<template>
  <h1 ref="greet">hi</h1>
  <p>App title</p>
  <Modal :header="header" :content="content" :theme="theme"/>
</template>

<script>
import Modal from "./components/Modal-m.vue" 
export default {

  data(){
    return{
      header:"Login in",
      content:"Welcome Kaung Min Khant",
      theme:"success"
    }
  },

  components:{
    Modal: Modal
  }
}
</script>

<style scoped>
h1{
  color:blue;
}
</style>