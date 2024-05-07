<template>
  <section>
    <h2 class="lg-text">People Love Cali Bookkeeping</h2>
    <div class="container">
      <div class="card">
        <div class="card-header">
          <p>Tony</p>
          <p>CEO</p>
          <span>
            <i class="fas fa-star" />
            <i class="fas fa-star" />
            <i class="fas fa-star" />
            <i class="fas fa-star" />
            <i class="fas fa-star" />
          </span>
        </div>
        <div class="card-body">
          <p>They provided excellent service and are transparent and honest in their charges.</p>
          <a href="/services/accounts-payable">
            View More
            <i class="fas fa-arrow-right" />
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  background-color: greenyellow;
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
  padding: 20px;
  gap: 20px;
}
h2 {
  text-align: center;
}
.container {
  display: flex;
  align-content: center;
  justify-content: center;
  flex-wrap: wrap;
  padding: 8px;
}
.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  border: solid 2px blue;
  border-radius: 5px;
  width: 200px;
}
.card-header {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  align-items: center;
  justify-items: center;
  background-color: lightblue;
  height: 50px;
}
.card-header span {
  grid-area: 2 / 1 / 3 / 3;
  color: yellow;
}

.card-body {
  display: flex;
  flex-direction: column;
  padding: 10px;
  gap: 20px;
  text-align: center;
}
a {
  font-size: 20px;
  align-self: flex-end;
}
</style>
