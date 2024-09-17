

<template>
  <main>
    <div>
      <h1>ERROR 404 - PAGE NON TROUVEE</h1>
      <p>La page que vous avez demandée n'existe pas</p>
    </div>
  </main>
</template>

<script setup>
import { useRoute } from 'vue-router';

const route = useRoute();

definePageMeta({
  title: 'Error 404 - Page non trouvée'
})

if (route.patch !== '*'){
  router.push({name: 'home'})
}
</script>



<style scoped>
</style>