<template>
  <div id="app">
    <Header />
    <main>
      <ProjectConfig />
      <Dependencies />
    </main>
  </div>
</template>

<script>
import Header from "../src/components/Header.vue";
import ProjectConfig from "../src/components/ProjectConfig.vue";
import Dependencies from "../src/components/Dependencies.vue";

export default {
  components: {
    Header,
    ProjectConfig,
    Dependencies,
  },
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  background: #eef0f1;
}
#app {
  display: flex;
  flex-direction: column;
  align-items: center;
}
main {
  display: flex;
  gap: 20px;
  padding: 20px;
}
</style>
