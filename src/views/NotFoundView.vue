<template>
  <div class="not-found-template">
    <div class="gh-outer">
      <div class="not-found-content">
        <h1>404</h1>
        <p>Page not found</p>
        <router-link to="/" class="btn">Go Home</router-link>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.not-found-content {
  text-align: center;
  padding: 4rem 0;
}

h1 {
  font-size: 6rem;
  margin-bottom: 1rem;
}

.btn {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  background: var(--ghost-accent-color, #050404);
  color: white;
  text-decoration: none;
  border-radius: 4px;
  margin-top: 1rem;
}
</style>
