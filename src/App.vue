<template>
  <Options />
  <Composition />
</template>

<script>
import Composition from "./components/compositionApi.vue";
import Options from "./components/optionsApi.vue";

export default {
  components: {
    Options,
    Composition,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
