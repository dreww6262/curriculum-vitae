<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import ContactCard from './components/ContactCard.vue'
</script>

<template>
  <div class="app-container">
    <div class="background-image-container">
      <img src="@/assets/providence.jpeg" class="background_image"/>
    </div>
    <div class="content">
      <header>
        
        <div class="wrapper">
          <ContactCard />

          <nav>
            <RouterLink to="/">Work Experience</RouterLink>
            <RouterLink to="/projects">Personal Projects</RouterLink>
            <RouterLink to="/about">About Me</RouterLink>
            <RouterLink to="/contact">Contact</RouterLink>
          </nav>
        </div>
      </header>

      <RouterView />
    </div>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

.app-container {
  width: 100%;
  height: 100%;
  place-items: center;
  margin: 0 auto;
}

.background_image_container {
  position: relative;
  overflow: hidden;
}

.background_image {
  min-height: 100%;
  min-width: 100%;
  opacity: 25%;
  position: absolute;
  top: 0;
  left: 0;
}

.content {
  height: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr;
  padding: 2rem;
  margin: 0 auto;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 1rem;
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

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }

  nav {
    text-align: center;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: .5rem;
  }
}
</style>
