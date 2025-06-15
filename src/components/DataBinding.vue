<template>
  <div class="container">
    <h1>{{ message }}</h1>
    <button @click="changeMessage">Change Message</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const message = ref("Hello, Vue 3!: Data Binding Example");

function changeMessage() {
  message.value = "Message updated!";
}
</script>

<style scoped>
.container {
  text-align: center;
  margin-top: 40px;
}

h1 {
  color: teal;
}

button {
  margin-top: 20px;
  padding: 8px 16px;
  font-size: 1rem;
}
</style>
