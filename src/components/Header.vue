<script setup lang="ts">
</script>

<template>
  <header>
    <div class="header-content">
      <h1>The Hub Hua Hin</h1>
      <nav>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>
</template>

<style scoped>
header {
  background-image: url('https://images.unsplash.com/photo-1527192491265-7e15c55b1ed2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80');
  background-size: cover;
  background-position: center;
  height: 300px;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.header-content {
  background-color: rgba(255, 255, 255, 0.8);
  padding: 20px;
  border-radius: 10px;
  text-align: center;
}

h1 {
  margin: 0;
  font-size: 32px;
  color: #333;
}

nav {
  margin-top: 10px;
}

nav a {
  margin: 0 10px;
  text-decoration: none;
  color: #333;
  font-weight: bold;
}

nav a:hover {
  color: #4CAF50;
}
</style>