<script setup>
import SingleCard from './SingleCard.vue';
import { ref } from 'vue';
</script>

<template>
  <div class="grid-container">
    <SingleCard />

    <SingleCard />
    <SingleCard />
  </div>
</template>

<style scoped>
.griid-container {
  display: flex; /* Activa Grid */
  flex-wrap: wrap;
  gap: 50px; /* Espacio entre las tarjetas */
  padding: 20px;
}
</style>
