<template>
  <section class="section-hero">
    <!-- text container -->
    <div class="hero-text-box">
      <h1 class="heading-primary">
        A healthy meal delivered to your door, every single day
      </h1>
      <p class="hero-desc">
        The smart 365-days-per-year food subscription that will make you eat
        healthy again. Tailored to your personal tastes and nutritional needs.
        We have delivered 250,000+ meals last year!
      </p>
    </div>
    <!-- image container -->
    <div class="hero-img-box">
      <img :src="imageBox" alt="hero image" />
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
