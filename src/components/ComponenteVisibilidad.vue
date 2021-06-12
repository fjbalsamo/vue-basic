<template>
  <div>
    <div v-if="visible">Hola soy un cartel</div>
    <div>
      <button @click="visible = !visible">
        {{ visible ? "Ocultar" : "Mostrar" }} 1
      </button>
    </div>
    <div>
      <button @click="toggle()">{{ visible ? "Ocultar" : "Mostrar" }} 2</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ComponenteVisibilidad",
  data() {
    return {
      visible: true,
    };
  },
  methods: {
    toggle() {
      this.visible = !this.visible;
    },
  },
};
</script>

<style></style>
