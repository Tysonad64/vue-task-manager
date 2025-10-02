<script setup lang="ts">
import { ref } from 'vue';

const newTask = ref('');

function formSubmitted() {
  console.log(newTask.value);
}
</script>

<template>
  <form @submit.prevent="formSubmitted">
      <label>
        New Task
        <input v-model="newTask" name="newTask">
      </label>
      <div class="button-container">
        <button type="submit">Add Task</button>
      </div>
    </form>
</template>

