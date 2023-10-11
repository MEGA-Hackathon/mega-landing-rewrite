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

@font-face {
  font-family: swiper-icons;
  src: url("data:application/font-woff;charset=utf-8;base64, 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") format("woff");
}

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