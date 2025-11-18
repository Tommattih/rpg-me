<script setup lang="ts">
import Map from './components/Map.vue'
import Card from './components/Card.vue'
</script>

<template>
  <h1>Tommattih.io</h1>
  <Card />
  <Map />

</template>

<style scoped>

h1 {
  margin: .5rem .5rem;
  color: white;
  font-size: 2.5rem;
}

.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
