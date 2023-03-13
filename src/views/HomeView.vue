<script setup>
import { count } from '../stores/counter'
const store = count()
</script>

<template>
  <main>
    <h1>Home view</h1>
    <h1>{{ store.number }}</h1>
    <button @click="store.increment()">ADD</button>
  </main>
</template>

<style scoped>
button {
  padding: 10px;
  background: greenyellow;
}
</style>
