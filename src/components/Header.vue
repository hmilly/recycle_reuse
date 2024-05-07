<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <header>
    <div class="title">
      <img src="@/assets/img/RR-logo.png" alt="Recycle, reuse. Home clearance experts" />
    </div>
    <nav>
      <RouterLink to="/"><p>Home</p></RouterLink>
      <RouterLink to="/contact"><p>Contact</p></RouterLink>
      <RouterLink to="/about"><p>About</p></RouterLink>
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
  text-align: center;
  gap: 10px;
}
nav a {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 5px;
  color: darkslategray;
}
nav a:hover {
  color: black;
  background-color: rgb(236, 238, 236);
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
