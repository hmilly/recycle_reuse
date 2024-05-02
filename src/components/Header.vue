<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <header>
    <div class="title">
      <img src="@/assets/img/RR-logo.png" alt="Recycle, reuse. Home clearance experts" />
    </div>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>
  </header>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-content: center;
  gap: 20px;
  border-bottom: 1px rgb(214, 214, 214) solid;
}
.title {
  display: flex;
  align-items: center;
}
.title img {
  min-width: 270px;
  max-width: 320px;
  height: 100%;
  width: auto;
}

nav {
  flex: 1;
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 12px;
  padding: 0 10px;
  text-align: center;
}
nav a {
  flex: 1;
  padding: 5px;
}

@media (max-width: 620px) {
  header {
    flex-direction: column;
  }
  .title {
    justify-content: center;
  }
}
</style>
