<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">
        <img alt="Vue logo" class="logo" src="@/assets/logo.png" width="125" height="125" />
      </RouterLink>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: inline-block;
  vertical-align: middle;
  margin-right: 1rem;
}

nav {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 12px;
  text-align: center;
  margin-top: 0.5rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

main {
  padding: 2rem;
}
</style>
