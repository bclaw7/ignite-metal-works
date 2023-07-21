<script setup>
import Home from './components/Home.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/ignite-metal-works-logo.png" width="280" height="280" />
  </header>

  <main>
    <Home />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

main {
  max-width: 800px;
  margin: 0 auto;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    justify-content: center;
  }
}
</style>
