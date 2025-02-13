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
.griid-container {
  display: flex; /* Activa Grid */
  flex-wrap: wrap;
  gap: 50px; /* Espacio entre las tarjetas */
  padding: 20px;
}
</style>
