<script setup>
import TitleComponent from './components/TitleComponent.vue'
</script>

<template>
  <header>
    <div>
      <TitleComponent />
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
  header {
    line-height: 1.5;
    max-height: 100vh;
  }
</style>
