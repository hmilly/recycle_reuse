<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <header>
    <div class="title">
      <h1>Recycle Reuse</h1>
    </div>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>
  </header>

</template>

<style scoped>
header{
  display: flex;
  justify-content: center;
  align-content: center;
  flex-wrap: wrap;
  padding: 5px 20px;
  margin-top: 10px;
  border-bottom: 1px rgb(214, 214, 214) solid;
}
.title {
  flex: 3;
}
.title,
h1 {
  display: inline-block;
}

nav {
  flex: 1;
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 12px;
  text-align: center;
}
nav a {
  padding: 5px;
}
</style>
