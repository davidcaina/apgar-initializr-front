<template>
  <button @click="toggleTheme">🌙/☀️</button>
</template>

<script>
export default {
  methods: {
    toggleTheme() {
      const currentTheme = document.body.classList.toggle("dark-mode");
      localStorage.setItem("theme", currentTheme ? "dark" : "light");
    }
  },
  mounted() {
    if (localStorage.getItem("theme") === "dark") {
      document.body.classList.add("dark-mode");
    }
  }
};
</script>

<style scoped>
button {
  cursor: pointer;
  background: transparent;
  border: none;
  font-size: 1.5rem;
}
</style>
