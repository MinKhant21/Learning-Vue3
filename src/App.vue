<template>
  <h1 ref="greet">hi</h1>
  <p>App title</p>
  <div v-if="showModal">
    <Modal :header="header" :content="content" :theme="theme" @close="showModal=false" />
  </div>
  <button @click="showModal=true">Open Modal</button>
  
</template>

<script>
import Modal from "./components/Modal-m.vue" 
export default {

  data(){
    return{
      header:"Login in",
      content:"Welcome Kaung Min Khant",
      theme:"success",
      showModal:false
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