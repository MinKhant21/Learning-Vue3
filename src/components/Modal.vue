<template>
  <div class="backdrop">
    <div class="modal">
        <p>Hi i am Modal component</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
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
</style>