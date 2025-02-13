<script setup>
defineProps ({item:Object})

</script>

<template>
  <div class="card">
    <img src="" alt="" class="card-img" />
    <div class="card-content">
      <img
        src="https://nfnatcane.es/blog/wp-content/uploads/2022/02/dos-cachorros-de-pastor-aleman-jugando.jpg"
        alt="12"
        class="card-img"
      />
      <h3>Raza: {{ item.raza }}</h3>
      <p><strong>Género:</strong> {{ item.genero }}</p>
      <p><strong>Estatura:</strong> {{ item.estatura }}</p>
      <p class="card-price">{{ item.precio }}</p>
      <button class="card-button">Más información</button>
    </div>
  </div>
</template>

<style scoped>
/* Estilo de la tarjeta */
.card {
  width: 300px;
  height: 360px;
  background-color: #ff6b6b;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  text-align: center;
  color: #fff;
  font-family: Arial, sans-serif;
}
/* Imagen dentro de la tarjeta */
.card-img {
  width: 100%;
  height: auto;
  max-height: 150px;
  object-fit: cover;
  border-bottom: 3px solid #fff;
}

.card-container {
  display: flex;
  gap: 20px;
  justify-content: space-around;
  padding: 0px;
  flex-wrap: wrap;
}
</style>
