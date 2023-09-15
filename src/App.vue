<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="hero-top">
      <img src='@/assets/fleekLogo.svg' height="87" />
      <img src='@/assets/plus.svg' />
      <img src='@/assets/logo.svg' height="57" />
    </div>

    <p className='description'>
      This is a template for creating a React site build it with Vite and deploying it on Fleek.
    </p>
  </header>

  <RouterView />
</template>

<style scoped>
template {
  display: flex;
  flex-direction: column;
}

header {
  display: flex;
  align-items: center;
  flex-direction: column;
  gap: 2.5rem;
}

.hero-top {
  display: flex;
  align-items: center;
  gap: 50px;
  margin-left: -95px;
}

.description {
  font-size: 1.5rem;
  line-height: 2rem;
  text-align: center;
  width: 100%;
}
</style>
