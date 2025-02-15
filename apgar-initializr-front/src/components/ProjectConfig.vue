<template>
  <div class="project-config">
    <h2>Project</h2>
    <div class="options">
      <label><input type="radio" v-model="projectType" value="maven" /> Maven</label>
      <label><input type="radio" v-model="projectType" value="gradle" /> Gradle</label>
    </div>

    <h2>Language</h2>
    <div class="options">
      <label><input type="radio" v-model="language" value="java" /> Java</label>
      <label><input type="radio" v-model="language" value="kotlin" /> Kotlin</label>
      <label><input type="radio" v-model="language" value="groovy" /> Groovy</label>
    </div>

    <h2>Spring Boot</h2>
    <select v-model="springBootVersion">
      <option value="3.4.2">3.4.2</option>
      <option value="3.3.9">3.3.9 (SNAPSHOT)</option>
      <option value="3.3.8">3.3.8</option>
    </select>

    <h2>Project Metadata</h2>
    <input type="text" v-model="group" placeholder="Group" />
    <input type="text" v-model="artifact" placeholder="Artifact" />
    <input type="text" v-model="description" placeholder="Description" />

  </div>
</template>

<script>
export default {
  data() {
    return {
      projectType: "maven",
      language: "java",
      springBootVersion: "3.4.2",
      group: "com.example",
      artifact: "demo",
      description: "Demo project for Spring Boot",
    };
  },
};
</script>

<style scoped>
.project-config {
  background: #fff;
  padding: 20px;
  border-radius: 5px;
}
.options label {
  margin-right: 10px;
}
</style>
