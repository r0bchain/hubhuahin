<script setup lang="ts">
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Slideshow from './components/Slideshow.vue'
import WhitelistForm from './components/WhitelistForm.vue'
</script>

<template>
  <div class="app">
    <Header />
    <Hero />
    <WhitelistForm />
    <Slideshow />
  </div>
</template>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
}

.app {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
</style>