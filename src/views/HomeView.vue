<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <main>
    <div class="d-grid gap-2 col-6 mx-auto mt-5">
      <RouterLink to="/library" class="btn btn-outline-danger">
        <span>LIBRERIA</span>
      </RouterLink>
      <RouterLink to="/flask" class="btn btn-outline-danger">
        <span>API FLASK</span>
      </RouterLink>
    </div>
  </main>
  <RouterView />
</template>
<style scoped>

</style>