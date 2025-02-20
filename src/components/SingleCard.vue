<template>
  <div class="tarjeta">
    <img :src="perro.imagen" :alt="perro.raza">
    <div class="contenido">
      <h3>Raza: {{ perro.raza }}</h3>
      <p><strong>Precio:</strong> {{ perro.precio }}</p>
      <button>Más información</button>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    perro: Object
  }
};
</script>

<style scoped>
.tarjeta {
  width: 200px;
  background-color: white;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
  text-align: center;
}

.tarjeta img {
  width: 100%;
  height: 120px;
  object-fit: cover;
}

.contenido {
  padding: 10px;
}

button {
  background-color: blue;
  color: white;
  border: none;
  padding: 10px;
  cursor: pointer;
  border-radius: 5px;
}
</style>
