<script>
export default {
  data() {
    return {
      name: 'Jake the Dog',
      status: false,
    }
  },
}
</script>

<template>
  <h1>Hello {{ name }}</h1>
  <p v-if="status">You're here!!!</p>
</template>

<style scoped></style>
