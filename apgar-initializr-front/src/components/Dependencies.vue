<template>
  <div class="dependencies">
    <h2>Dependencies</h2>
    <button @click="openModal">ADD DEPENDENCIES...</button>
  </div>
</template>

<script>
export default {
  methods: {
    openModal() {
      alert("Abrir modal para selecionar dependências");
    },
  },
};
</script>

<style scoped>
.dependencies {
  background: #f8f9fa;
  padding: 20px;
  border-radius: 5px;
}
button {
  padding: 10px;
  cursor: pointer;
}
</style>
