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
  max-height: 3rem;
  max-width: 3rem;
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
}

nav a {
  color: #6a5dd8;
  text-decoration: none;
  margin-left: 1rem;
  font-size: 1rem;
  transition: color 0.3s;
}

nav a:hover {
  color: #4b3bbd;
  background-color: transparent; /* 背景色を透明に設定 */
}

main {
  padding: 5rem 2rem 2rem;
  max-width: 1200px;
  margin: 0 auto;
}
</style>
