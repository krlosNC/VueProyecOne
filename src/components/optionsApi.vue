<template>
  <h2>Options API</h2>
  <h3>Coche</h3>
  <p>Marca: {{ marca }}</p>
  <p>Modelo: {{ modelo }}</p>
  <p>Color: {{ color[0] }}</p>
  <p>Precio: {{ precio }}</p>
  <p>Potencia: {{ poder }} hp</p>

  <button @click="maxPoder">Aumentar</button>
  <button @click="minPoder">Disminuir</button>
</template>

<script>
export default {
  data() {
    return {
      marca: "Audi",
      modelo: "4A",
      color: ["azul", "rojo", "verde"],
      precio: 38500,
      poder: 50,
    };
  },

  methods: {
    maxPoder() {
      this.poder++;
    },
    minPoder() {
      this.poder--;
    },
  },
};
</script>

<style>
button {
  cursor: pointer;
  margin: 0px 10px;
}
</style>
