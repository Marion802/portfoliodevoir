<template>
<premierepartie/>

  <footer id="pied" class="roseclair">

      <a target="_blank" href="https://github.com/Marion802"><img src="/src/assets/logo-github.png" alt="logo-github"></a>
      <a target="_blank" href="https://www.linkedin.com/in/marion-sermande-1a3208307/"><img src="/src/assets/linkedin.png" alt="logo-linkedin"></a>
      <a target="_blank" href="https://x.com/MarionSermande"><img src="/src/assets/twitter.png" alt="logo-twitter"></a>
      <p><small>Mise à jour le <time datetime="2024-18-09"> 18 septembre 2024</time></small></p>


    </footer>



</template>




<script setup>

import premierepartie from './components/HelloWorld.vue';

import present from '@/App.vue'

import formulaire from './components/HelloWorld.vue';

const form = document.getElementById (formulaire);


</script>





<style scoped>

.roseclair {
  background-color: #ffa9f9;
}

small {
  margin-left: 50%;
}

#pied img {
  width: 50px;
  height: 50px;
  margin-left: 25%;
}

</style>


