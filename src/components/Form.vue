<template>
  <form @submit="onSubmit" class="contact-form">
    <h3>Get an Estimate</h3>
    <div class="form-control">
      <input type="text" v-model="name" autoComplete="given-name" id="name" value="" />
      <label>Name</label>
    </div>
    <div class="form-control">
      <input type="text" v-model="email" required id="email" value="" />
      <label>Email*</label>
    </div>
    <div class="form-control">
      <input type="text" v-model="address" id="address" value="" required />
      <label> Property address </label>
    </div>

    <div class="form-control">
      <select id="size" v-model="size" value="" name="size">
        <option>Small (1 bedroom)</option>
        <option>Medium (2-3 bedrooms)</option>
        <option>Large (5+ bedrooms)</option>
      </select>
      <label for="size">Property size</label>
    </div>
    <div class="form-control">
      <input type="number" v-model="sqFoot" required id="sqFoot" value="" />
      <label> Sq foot to be cleaned (number) </label>
    </div>
    <textarea
      type="text"
      v-model="description"
      value=""
      id="description"
      placeholder="Tell us more about your cleaning needs so we can give you a more accurate estimate."
    />
    <button type="submit" aria-label="Submit">Send</button>
    <div class="form-terms">
      <p>
        This site is protected by reCAPTCHA and the
        <a
          href="https://policies.google.com/privacy"
          target="_blank"
          rel="noreferrer"
          aria-label="google privacy statement"
        >
          Google Privacy Policy
        </a>
        and
        <a
          href="https://policies.google.com/terms"
          target="_blank"
          rel="noreferrer"
          aria-label="google terms"
        >
          Terms of Service.
        </a>
      </p>
    </div>
  </form>
</template>

<script>
export default {
  name: 'user',
  data() {
    return {
      name: '',
      email: '',
      address: '',
      size: '',
      sqFoot: '',
      description: ''
    }
  },
  methods: {
    onSubmit(e) {
      e.preventDefault()

      if (!this.email) {
        alert('Please add more details')
        return
      }

      const newUser = {
        // id: Math.floor(Math.random() * 100000),
        name: this.name,
        email: this.email,
        address: this.address,
        size: this.size,
        sqFoot: this.sqFoot,
        description: this.description
      }

      this.name = ''
      this.email = ''
      this.address = ''
      this.size = ''
      this.sqFoot = ''
      this.description = ''
    }
  }
}
</script>

<style scoped>
form {
  margin: 0 auto;
  flex: 1;
  max-width: 600px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  padding: 10px;
  gap: 10px;
}
.form-control {
  height: 90px;
  width: 100%;
  position: relative;
}
input,
select {
  position: absolute;
  border: solid 1px black;
  width: 100%;
  height: 60px;
  left: 0;
  padding: 15px 20px 5px 20px;
}

input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}
.active {
  background-color: aqua;
}
label {
  position: absolute;
  bottom: 50px;
  left: 20px;
  font-size: 1em;
  transition: 0.6s;
}
input:focus ~ label,
.inputFilled {
  transform: translateX(-10px) translateY(-20px);
  font-size: 0.8em;
}
textarea {
  width: 100%;
  height: 200px;
  padding: 10px;
  margin-bottom: 15px;
  resize: none;
}
button {
  color: black;
  width: 90%;
  height: 50px;
  margin: 0 auto;
  margin-bottom: 15px;
}
.form-terms {
  text-align: center;
  padding-bottom: 20px;
}
.form-terms a {
  display: inline;
}

@media only screen and (max-width: 350px) {
  h3 {
    text-align: center;
  }
}
</style>
