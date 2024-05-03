<template>
  <section class="home"></section>

  <section class="services">
    <h2>SERVICES</h2>
    <div class="description">
      <p>
        At Recycle Reuse, we offer comprehensive services tailored to meet the diverse needs of our
        clients.
      </p>
      <p>
        we believe in offering competitive and transparent pricing to our clients. Our pricing
        structure is based on the volume and type of items being cleared, ensuring fair and
        affordable rates for our services.
      </p>
      <p id="bold-text">Contact us today for a free quote tailored to your specific needs.</p>
    </div>
  </section>
</template>

<style scoped>
.home {
  width: 100%;
  height: auto;
  min-height: 400px;
  display: flex;
  justify-content: center;
  align-content: center;
  background-image: url('@/assets/img/clean_home.jpg');
  background-position: center;
  background-size: cover;
}
.home h2 {
  max-width: 600px;
  height: auto;
  margin-top: 40px;
  text-align: center;
}
.services {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 30px;
  gap: 20px;
}

.description {
  max-width: 600px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  gap: 16px;
  padding: 16px;
}
</style>
