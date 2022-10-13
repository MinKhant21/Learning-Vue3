<template>
  <h1 ref="greet">hi</h1>
  <Modal/>
</template>

<script>
import Modal from './components/Modal.vue'
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
  },
  components:{
    Modal:Modal
  }
}
</script>

<style>
h1{
  color:blue;
}
</style>