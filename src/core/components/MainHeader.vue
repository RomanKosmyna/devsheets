<script setup lang="ts">
import { RouterLink } from 'vue-router'
import MainLogo from './MainLogo.vue';
</script>

<template>
  <header>
    <div class="pWrapper">
      <div class="innerWrapper">
        <MainLogo />
        <div class="navWrapper">
          <nav>
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/sheets">Sheets</RouterLink>
          </nav>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
header {
  line-height: 1.5;
  width: 100%;
  height: 4.5rem;
  background-color: red;
  background: rgba(0, 0, 0, 0.7);
  backdrop-filter: blur(6px);
}

.pWrapper {
  width: 100%;
  height: 100%;
  padding: 0 1.25rem;
}

.innerWrapper {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 5rem;
}

.navWrapper {
  height: 100%;
  display: flex;
  justify-content: end;
}

nav {
  display: flex;
  height: 100%;
  font-size: 12px;
  text-align: center;
  align-items: center;
}

nav a.router-link-exact-active {
  color: #FFEABF;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  font-size: 1.3rem;
  font-weight: 500;
  color: #BFAF8F;
}

nav a:not(.router-link-exact-active):hover {
  color: #FFEABF;
}

nav a:first-of-type {
  border: 0;
}

/* @media (min-width: 1024px) {
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
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
} */
</style>
