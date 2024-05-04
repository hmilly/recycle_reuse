<template>
  <div class="container">
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-home" />
      </div>
      <p id="lg-text">Full House Clearance</p>
      <p>
        Our flagship service involves clearing out entire properties, leaving them completely empty
        and ready for the market. Whether you're downsizing, relocating, or preparing a property for
        sale, we handle the entire process efficiently and professionally.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-door-open" />
      </div>
      <p id="lg-text">Room Clearances</p>
      <p>
        If you're renovating a room or transitioning a space, our room clearance service is the
        perfect solution. We'll clear out unwanted items, allowing you to start fresh and transform
        your space according to your vision.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-couch" />
      </div>
      <p id="lg-text">Single Item Removal</p>
      <p>
        Need to declutter your space or dispose of a specific item? We're here to help. From bulky
        furniture to appliances and electronics, we can remove individual items with ease, saving
        you time and effort.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-recycle" />
      </div>
      <p id="lg-text">Eco-Friendly Disposal</p>
      <p>
        As advocates for sustainability, we prioritise eco-friendly disposal methods. Items that
        cannot be resold are recycled or donated to local charities, minimising landfill waste and
        promoting a greener future.
      </p>
    </div>
  </div>
</template>

<style scoped>
.container {
  max-width: 800px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding: 16px 0;
  gap: 16px;
}
.card {
  width: 350px;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  background-color: rgb(207, 252, 224);
  border: solid 1px black;
  transition-duration: 300ms;
  border-radius: 10px;
  padding: 20px;
  margin-right: 15px;
  gap: 30px;
}
.card:hover {
  cursor: pointer;
  background-color: rgb(211, 252, 207);
}
.card_logo {
  width: 100px;
  height: 100px;
  background-color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  border: solid 2px darkgreen;
}
.fas {
  font-size: 50px;
  color: green;
}
</style>
