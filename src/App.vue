<script setup>
import { ref } from 'vue'
import { RouterLink, RouterView } from 'vue-router'
const isHovered = ref(false)
</script>

<template>
  <div class="app">
    <header class="header">
      <div class="logo">
        <img src="./assets/download.png" />
      </div>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/contact-us">Contact Us</RouterLink>
        <button
          @mouseover="isHovered = true"
          @mouseleave="isHovered = false"
          :class="{ 'button-hover': isHovered }"
        >
          Get Demo
        </button>
      </nav>
    </header>
    <RouterView />
  </div>
</template>

<style scoped>
.app {
  font-family: Arial, sans-serif;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}

.logo {
  width: 150px;
  height: 150px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 24px;
  font-weight: bold;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a {
  display: inline-block;
  padding: 0 2rem;
  border-left: 1px solid var(--color-border);
}

.button-hover {
  background-color: white;
}

button {
  background-color: lightskyblue;
  color: black;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.5s ease;
}
</style>
