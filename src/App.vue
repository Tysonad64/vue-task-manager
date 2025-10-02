<script setup lang="ts">
import { ref } from 'vue';

const message = ref('Tasks Manager');
const newTask = ref('');
</script>

<template>
  <main>
    <h1>{{ message }}</h1>
    <form>
      <label>
        New Task
        <input v-model="newTask" name="newTask">
      </label>
      <div class="button-container">
        <button type="submit">Add Task</button>
      </div>
    </form>
  </main>
</template>

<style scoped>
main {
  max-width: 800px;
  margin: 1rem auto;
}

.button-container {
  display: flex;
  justify-content: end;
}
</style>
