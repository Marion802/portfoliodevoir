<template>
    <div id="Comment">

          

        <div class="modal">
        <div class="overlay" @click="$emit('close')"></div>
        <div class="modal-container">
        <button class="close-button" @click="$emit('close')">X</button>
        <slot></slot>
        <a href=""><img src="" alt=""></a>
        </div>
        </div>
    </div>


</template>

<script setup>
name : "Comment"
</script>

<style scoped>
.modal {
  position: fixed;
  top: 0;
  width: 100%;
  height: 100vh;
}

.close-button {
  position: absolute;
  top: 0;
  right: 0;
}


.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  background: #333333d3;
}

.modal-container{
  width: 95%;
  height: 600px;
  max-width: 900px;
  min-width: 300px;
  padding: 50px;
  background: pink;
  border-radius: 5px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}


</style>