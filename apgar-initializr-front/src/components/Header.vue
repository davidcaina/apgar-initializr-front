<template>
  <header class="header">
    <img src="" alt="Spring Initializr Logo" />
    <h1>Spring Initializr</h1>
    <ThemeToggle />
  </header>
</template>

<script>
import ThemeToggle from "./ThemeToggle.vue";
export default {
  components: { ThemeToggle },
};
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem;
  background: #fff;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}
</style>
