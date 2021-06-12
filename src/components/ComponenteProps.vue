<template>
  <div>
    <h5>hola mi prop es: {{ saludo }}</h5>
    <h5>nombre: {{ nombre }}</h5>
  </div>
</template>

<script>
export default {
  name: "ComponenteProps",
  props: {
    saludo: String,
    nombre: {
      type: String,
      default: "Juan",
    },
  },
};
</script>

<style></style>
