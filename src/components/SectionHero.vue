<template>
  <section class="section-hero">
    <div class="hero">
      <!-- text container -->
      <div class="hero-text-box">
        <h1 class="heading-primary">
          A healthy meal delivered to your door, every single day
        </h1>
        <p class="hero-description">
          The smart 365-days-per-year food subscription that will make you eat
          healthy again. Tailored to your personal tastes and nutritional needs.
          We have delivered 250,000+ meals last year!
        </p>
        <!-- add router-link -->
        <a href="#" class="btn">Start eating well</a>
        <a href="#" class="btn">Learn more &darr;</a>
      </div>
      <!-- image container -->
      <div class="hero-img-box">
        <img
          :src="imageBox"
          alt="Woman enjoying food, meals in storage container, and food bolws on a table"
          class="hero-img"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      imageBox: require('../assets/images/hero.png'),
    };
  },
};
</script>

<style scoped>
.hero-img {
  /* Image container is 100% filled */
  width: 100%;
}
.section-hero {
  background-color: #fdf2e9;
}
.hero {
  align-items: center;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  max-width: 110rem;
  margin: 0 auto;
}

.heading-primary {
  color: #333;
  font-size: 5.2rem;
  font-weight: 700;
  letter-spacing: -0.5px;
  line-height: 1.05;
  margin: 0 0 3.2rem 0;
}
.hero-description {
  font-size: 2rem;
  line-height: 1.5;
  margin: 0 0 4.8rem 0;
}
</style>
