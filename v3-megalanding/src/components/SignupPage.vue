<template>
  <div>
    <div class="signup-page">
      <h2>Subscribe to get notified about new events</h2>
      <p>We won't send spam!</p>
      <input type="email" v-model="email" @input="validateEmail" placeholder="Enter your email">
      <button @click="subscribe">Subscribe</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email : '',
    };
  },
  methods: {
    validateEmail() {
    },
  },
}
</script>

<style scoped>
.signup-page {
  position: absolute;
  background-color: #000;
  width: 85rem;
  height: 25rem;
}

.signup-page h2 {
  position: relative;
  font-size: 30px;
  color: #fff;
  margin-top: 100px;
}

.signup-page p{
  color: grey;
}

.signup-page input {
  width: 24rem;
  height: 4rem;
  margin: 40px 20px 0 0;
  background-color: #282626;
  border: none;
  font-size: 18px;
  padding-left: 20px;
  border-radius: 8px;
}

.signup-page button {
  background-color: #fff;
  color: #000;
  width: 9rem;
  height: 4rem;
  font-size: 20px;
  border-radius: 8px;
}

@media (max-width: 1024px){
    .signup-page {
      width: 100%;
      height: 60%;
  }

  .signup-page h2 {
    font-size: 22px;
    width: 75%;
    margin-left: 90px;
  }
}

@media (max-width: 760px) {
  .signup-page {
    width: 100%;
    height: 80%;
  }

  .signup-page h2 {
    font-size: 25px;
    width: 75%;
    margin-left: 60px;
  }

  .signup-page input {
    width: 80%;
    height: 3.5rem;
    margin-left: 17px;
  }

  .signup-page button {
    width: 85%;
    height: 3.5rem;
    margin-top: 10px;
  }
}

</style>