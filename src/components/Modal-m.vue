<template>
  <div class="backdrop" @click.self="closeModal">
    <div class="modal" :class="{success:theme=='success'}">
        <h1>{{ header }}</h1>
        <p>{{ content }}</p>
       
    </div>
  </div>
</template>

<script>
export default {
  props:['header','content','theme'],
  methods:{
    closeModal()
    {
      this.$emit("close")
    }
  }
}
</script>

<style scoped>
.h1{
  color:rgb(23, 22, 23);
}
.backdrop{
    position:fixed;
    top: 0;
    background-color: rgba(0, 0, 0,0.5);
    width: 100%;
    height: 100%;
}
.modal{
  width: 400px;
  padding: 20px;
  margin: 100px auto;
  border-radius: 10px;
  background-color: white;
}
P{
  font-style: normal;
}
.success{
  background-color: green;
  color: white;
  text-align: center;
}
.delete{
  background-color: crimson;
  color: white;
  text-align: center;
}
</style>