<script setup>
import { ref } from 'vue'

// declare reactive variables
const name = ref('Jake the Dog')
const status = ref(true)

function change() {
  status.value = !status.value
}
</script>
<template>
  <div class="condtiom-directives">
    <h1>Hello {{ name }}</h1>
    <p v-if="status === true">User is Avtive</p>
    <p v-else>User is not active</p>
    <button @click="change">Click to Switch</button>
  </div>
</template>

<style scoped>
p {
  font-size: 3rem;
}
</style>
