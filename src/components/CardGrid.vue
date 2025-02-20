<template>
  <div class="tarjetas-container">
    <DogCard v-for="(perro, index) in perros" :key="index" :perro="perro" />
  </div>
</template>

<script>
import DogCard from './DogCard.vue';

export default {
  components: { DogCard },
  data() {
    return {
      perros: [
        { raza: "Pug", imagen: "url_del_pug", precio: "1.100.000 - 1.500.000" },
        { raza: "Poodle", imagen: "url_del_poodle", precio: "1.100.000 - 7.000.000" },
        { raza: "Golden", imagen: "url_del_golden", precio: "1.400.000" },
        // Agrega todas las razas aquí
      ]
    };
  }
};
</script>

<style scoped>
.tarjetas-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
  padding: 20px;
}
</style>
