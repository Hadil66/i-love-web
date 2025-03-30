<script setup>
  import Marchnotes from './components/Marchnotes.vue';
</script>

<template>
  <header>
    <h1> I love web</h1>
  </header>

  <main>
    <Marchnotes />
  </main>
</template>

<style scoped>
template {
  background-color: hsl(75, 36%, 38%);
}

header h1 {
  color: var(--dark-clr-10);
}
</style>
