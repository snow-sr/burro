<script setup>
import dog from "./components/dog.vue";
</script>

<template>
  <main class="mapa">
    <dog name="fumaça" :position="[230, 240]"></dog>
    <dog name="Maicon" :position="[540, 600]"></dog>
  </main>
</template>

<style scoped>
/* Background image assets/mapa */
.mapa {
  background-image: url("./assets/ifcmapatt.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  height: 100vh;
  width: 100vw;
}
</style>
