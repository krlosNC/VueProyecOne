<template>
  <h2>Composition API</h2>
  <h3>Coche</h3>
  <p>Marca: {{ marca }}</p>
  <p>Modelo: {{ modelo }}</p>
  <p>Color: {{ color[2] }}</p>
  <p>Precio: {{ precio }}</p>
  <p>Potencia: {{ poder }} hp</p>

  <button @click="maxPoder">Aumentar</button>
  <button @click="minPoder">Disminuir</button>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const marca = "Audi";
    const modelo = "4A";
    const color = ["azul", "rojo", "verde"];
    const precio = 38500;
    let poder = ref(180);

    const maxPoder = () => {
      poder.value++;
    };
    const minPoder = () => {
      poder.value--;
    };

    return {
      marca,
      modelo,
      color,
      precio,
      poder,
      maxPoder,
      minPoder,
    };
  },
};
</script>

<style>
button {
  cursor: pointer;
  margin: 0px 10px;
}
</style>
