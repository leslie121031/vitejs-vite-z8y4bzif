<script setup>
import SingleCard from './SingleCard.vue';
import { ref } from 'vue';
import {database} from '../database/database'

console.log(database)

const items = ref(database)

</script>

<template>
  <div class="grid-container">
    <SingleCard v-for="item in items" :item="item"/>
  </div>
</template>


<style scoped>
.grid-container {  /* ← Aquí estaba mal escrito como griid-container */
  display: flex;
  flex-wrap: wrap;
  gap: 20px; /* Ajusta este valor si siguen muy juntas */
  padding: 20px;
  justify-content: center; /* Centra las tarjetas */
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}

</style>
