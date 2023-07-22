<script setup>
import Home from './components/Home.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/ignite-metal-works-logo.png" width="280" height="280" />
    <div class="contact-info">
      <a href="tel:8067781029" class="hover-underline-animation">&#9742; (806)778-1029</a>
      <a href="mailto:chase@ignitemetalworks.com" class="hover-underline-animation">&#128231; ignitemetalworks.com</a>
    </div>
  </header>

  <main>
    <Home />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  display: flex;
  flex-wrap: wrap-reverse;
}

main {
  max-width: 800px;
  margin: 0 auto;
}

.logo {
  display: block;
  margin: 0 auto;
}

.contact-info {
  display: flex;
  justify-content: space-between;
  width: 100%;
  padding-top: 1rem;
}

.hover-underline-animation {
  display: inline-block;
  position: relative;
}

.hover-underline-animation::after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: var(--color-heading);
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
}

.hover-underline-animation:hover::after {
  transform: scaleX(1);
  transform-origin: bottom left;
}

@media screen and (min-width: 1024px) {
  header {
    flex-wrap: nowrap;
  }

  .contact-info {
    width: auto;
    justify-content: space-evenly;
    flex-direction: column;
  }

}
</style>
