<template>
  <header class="header">
    <img src="../../public/header-logo.png" alt="Spring Initializr Logo" class="logo" />
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
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
}

.logo {
  height: 50px;
  margin-left: 1rem;
}
</style>
