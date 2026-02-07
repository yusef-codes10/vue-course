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
  <h1>Hello {{ name }}</h1>
  <p v-if="status">You're here!!!</p>
  <p v-else>You are not here</p>
  <button @click="change">Click to Switch</button>
</template>

<style scoped></style>
