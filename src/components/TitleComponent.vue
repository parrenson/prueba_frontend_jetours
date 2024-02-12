<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

const textForRoute = () => {
  switch (router.currentRoute.value.path) {
    case "/":
        return "En esta web podrás probar la funcionalidad de las diferentes API que se incluyen en la prueba técnica, para ello, selecciona la opción que desees probar en el menú de navegación.";
      break;
    case "/library":
      return "En esta sección podrás buscar libros por título, autor o ISBN. También podrás ver los detalles de un libro en concreto.";
      break;
    case "/flask":
      return "En esta sección podrás probar la API de Flask, que incluye un endpoint para obtener la lista de libros y otro para obtener los detalles de un libro en concreto.";
      break;
    default:
      break;
  }
}
</script>

<template>
  <div class="">
    <h1 class="fw-bold text-center mb-5">
        <span class="text-dark">Prueba técnica </span>
        <span class="text-danger">JE TOURS</span>
    </h1>
    <h3 class="fw-bold text-center mb-2">
      <span class="text-dark info">
        {{ textForRoute() }}
      </span>
    </h3>
  </div>
</template>

<style scoped>
h1 {
  position: relative;
}

h3 {
  font-size: 1.2rem;
}

</style>
