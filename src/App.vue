<template>
  <div class="app-container">
    <header>
      <h1>Sofi's Pet Shop</h1>
    </header>

    <main>
      <CardGrid />
    </main>

    <footer>
      <p>&copy; 2025 Sofi's Pet Shop - Todos los derechos reservados.</p>
    </footer>
  </div>
</template>

<script>
import CardGrid from "./components/CardGrid.vue";

export default {
  components: { CardGrid }
};
</script>

<style scoped>
/* Estilos para el Header */
header {
  background-color: #ff69b4; /* Color rosa fuerte */
  color: white;
  text-align: center;
  padding: 15px;
  font-size: 1.5rem;
}
body {
  background-color: #87CEEB; /* Azul celeste */
  margin: 0;
  font-family: Arial, sans-serif;
}

/* Estilos para el Footer */
footer {
  background-color: #333; /* Color oscuro */
  color: white;
  text-align: center;
  padding: 10px;
  margin-top: 20px;
}
</style>

