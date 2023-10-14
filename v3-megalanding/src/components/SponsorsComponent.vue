<template>
  <section>
    <img class="main-image" src="../assets/sponsors.png" alt="Sponsors & Partners" />
    <div class="main-container">
      <h3 class="title">Sponsors & Partners</h3>
      <div class="container">
        <div class="sub-container">
          <img class="sub-image" src="../assets/person.png" alt="Diverse & Connected" />
          <div class="text-container">
            <h3 class="subtitle text">Diverse & Connected</h3>
            <p class="text">Our sponsors span the globe in multiple continents and support our efforts and chapters globally, providing funding and helping raise capital for our next ventures.</p>
          </div>
        </div>
        <div class="sub-container">
          <img class="sub-image" src="../assets/light.png" alt="Opportune" />
          <div class="text-container">
            <h3 class="subtitle text">Opportune</h3>
            <p class="text">Our sponsors provide guest speakers and years of experience to MEGA Events which truly make
              them MEGA.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,400;0,9..40,500;0,9..40,600;0,9..40,700;1,9..40,400;1,9..40,500;1,9..40,600&display=swap');

html, body, h1, h3, p {
  font-family: 'DM Sans', sans-serif;
  width: 100%;
  height: 100%;
  margin: 0;
}

h1, h3 {
  color: #0F2137;
  font-weight: 700;
}

p {
  color: #343D48;
  line-height: 1.73;
}

.title {
  font-size: 23px;
  letter-spacing: -1.5px;
  text-align: center;
}

.subtitle {
  letter-spacing: -0.5px;
  font-size: 18px;
}

section {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 20px;
}

.main-image {
  max-width: 100%;
  float: right;
}

.main-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 30px;
  padding: 20px 30px;
}

.sub-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 10px;
  padding: 30px;
}

.sub-image {
  margin-bottom: 10px;
}

.text-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 10px;
}

.text {
  text-align: center;
}

@media (min-width: 768px) {
  .title {
    font-size: 30px;
  }

  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
  }

  .sub-container {
    flex-direction: row;
    align-items: start;
    gap: 30px;
  }

  .text-container {
    align-items: start;
  }

  .text {
    text-align: start;
  }
}

@media (min-width: 1200px) {
  section {
    width: 100%;
    margin: auto;
    flex-direction: row;
    align-items: start;
    min-height: min-content;
    gap: 20px;
    padding: 0px 30px;
  }

  .title {
    font-size: 36px;
    text-align: start;
  }

  .main-container {
    padding: 0px;
    max-width: 40%;
    min-height: 100%;
  }

  .container {
    flex-direction: column;
  }

  .sub-container {
    padding: 15px 40px;
  }

  .main-image {
    max-width: 60%;
    min-height: 100%;
  }

  .title {
    padding-top: 60px;
    margin-left: 50px;
  }
}
</style>