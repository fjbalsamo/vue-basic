<template>
  <div id="app">
    <h1>Hola soy App.vue</h1>
    <ComponenteSimple key="cs1"></ComponenteSimple>
    <ComponenteSimple key="cs2" />
    <hr />
    <ComponenteLogica />
    <hr />
    <ComponenteReactivo />
    <hr />
    <ComponenteReactivo />
    <hr />
    <ComponenteVisibilidad />
    <hr />
    <componente-visibilidad />
    <ComponenteProps saludo="saludo CP1" />
    <hr />
    <ComponenteProps saludo="saludo CP2" :nombre="nombre" />
    <button @click="nombre = 'Alex'">click</button>
  </div>
</template>

<script>
import ComponenteSimple from "./components/ComponenteSimple.vue";
import ComponenteLogica from "./components/ComponenteLogica.vue";
import ComponenteReactivo from "./components/ComponenteReactivo.vue";
import ComponenteVisibilidad from "./components/ComponenteVisibilidad.vue";
import ComponenteProps from "./components/ComponenteProps.vue";

export default {
  name: "App",
  components: {
    ComponenteSimple,
    ComponenteLogica,
    ComponenteReactivo,
    ComponenteVisibilidad,
    ComponenteProps,
  },
  data() {
    return {
      nombre: "Gloria",
    };
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
  margin-top: 60px;
}
</style>
