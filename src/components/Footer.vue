<template>
    <div class="copyright">
        <img src="../assets/ignite-metal-works-logo.png" class="logo" alt="Ignite Metal Works logo">
        <p>&copy; 2023 Ignite Metal Works, LLC.</p>
    </div>
</template>

<style scoped>
.copyright {
    color: var(--black);
    max-width: 600px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: auto;
}

.logo {
    width: 100px;
    height: auto;
}

@media (min-width: 1024px) {
    .logo {
        width: 200px;
    }
}
</style>