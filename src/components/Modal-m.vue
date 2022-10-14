<template>
  <div class="backdrop">
    <div class="modal" :class="{success:theme=='success'}">
        <h1>{{ header }}</h1>
        <p>{{ content }}</p>
       
    </div>
  </div>
</template>

<script>
export default {
  props:['header','content','theme']
}
</script>

<style scoped>
.h1{
  color:rgb(23, 22, 23);
}
.backdrop{
    position:fixed;
    background-color: bisque;
    width: 100%;
    height: 100%;
}
.modal{
    background-color: white;
    padding: 100px auto;
    margin: 100px auto;
   
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