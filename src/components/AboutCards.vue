<template>
  <div class="container">
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-recycle" />
      </div>
      <p id="lg-text">Sustainability</p>
      <p>
        We are committed to minimising waste and maximising reuse through eco-friendly practices,
        promoting a greener future for generations to come.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-balance-scale" />
      </div>
      <p id="lg-text">Integrity</p>
      <p>
        We conduct our business with honesty, transparency, and ethical principles, earning the
        trust and respect of our clients and communities.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-handshake" />
      </div>
      <p id="lg-text">Professionalism</p>
      <p>
        We uphold the highest standards of professionalism in all aspects of our operations,
        ensuring a seamless and reliable experience for our clients.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-calendar-alt" />
      </div>
      <p id="lg-text">Flexibility</p>
      <p>
        We recognise the unique needs of each client and adapt our services accordingly, offering
        flexible options to accommodate diverse requirements and preferences.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-clipboard-check" />
      </div>
      <p id="lg-text">Accountability</p>
      <p>
        We take ownership of our actions and outcomes, holding ourselves accountable to deliver
        results with excellence and reliability.
      </p>
    </div>
    <div class="card">
      <div class="card_logo">
        <i class="fas fa-hand-holding-heart" />
      </div>
      <p id="lg-text">Community Engagement</p>
      <p>
        We actively engage with and give back to our local communities, supporting charitable
        initiatives and fostering positive social impact.
      </p>
    </div>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
  max-width: 800px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding: 16px 0;
  gap: 16px;
}
.card {
  width: 250px;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  border: solid 1px rgb(207, 252, 224);;
  transition-duration: 300ms;
  border-radius: 10px;
  padding: 20px;
  gap: 20px;
}
.card:hover {
  background-color: rgb(207, 252, 224);
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
