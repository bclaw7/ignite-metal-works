<script setup>
import Hero from './components/Hero.vue'
import Home from './components/Home.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <header>
    <Hero />
  </header>
  <main>
    <Home />
  </main>
  <footer>
    <Footer />
  </footer>
</template>

<style scoped>
main {
  padding: 0 1rem;
}

footer {
  background-color: var(--white);
  padding: 1rem;
  clip-path: polygon(0 0, 100% 13%, 100% 100%, 0 100%);
}

@media (min-width: 1024px) {
  footer {
    clip-path: polygon(0 0, 100% 23%, 100% 100%, 0 100%);
  }
}
</style>