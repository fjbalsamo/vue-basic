<template>
  <div>
    <input
      type="text"
      id="nombre"
      placeholder="nombre"
      v-model="name"
      autocomplete="off"
    />
    <h4>{{ name }}</h4>
  </div>
</template>

<script>
export default {
  name: "ComponenteReactivo",
  data() {
    return {
      name: "Pedro",
    };
  },
};
</script>

<style></style>
