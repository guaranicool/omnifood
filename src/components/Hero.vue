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
          We have delivered
        </p>
        <!-- add router-link -->
        <a href="#" class="btn btn-full margin-right-sm">Start eating well</a>
        <a href="#" class="btn btn--outline">Learn more &darr;</a>

        <div class="delivered-meals">
          <div class="delivered-imgs">
            <img :src="deliveredImgA" alt="Customer photo" />
            <img :src="deliveredImgB" alt="Customer photo" />
            <img :src="deliveredImgC" alt="Customer photo" />
            <img :src="deliveredImgD" alt="Customer photo" />
            <img :src="deliveredImgE" alt="Customer photo" />
            <img :src="deliveredImgF" alt="Customer photo" />
          </div>
          <p class="delivered-text">
            <span>250,000+</span> meals delivered last year!
          </p>
        </div>
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
      deliveredImgA: require('../assets/images/customers/customer-1.jpg'),
      deliveredImgB: require('../assets/images/customers/customer-2.jpg'),
      deliveredImgC: require('../assets/images/customers/customer-3.jpg'),
      deliveredImgD: require('../assets/images/customers/customer-4.jpg'),
      deliveredImgE: require('../assets/images/customers/customer-5.jpg'),
      deliveredImgF: require('../assets/images/customers/customer-6.jpg'),
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
  padding: 9.6rem 0;
}
.hero {
  align-items: center;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 9.6rem;
  max-width: 120rem;
  margin: 0 auto;
}
.delivered-meals {
  display: flex;
  align-items: center;
  gap: 1.6rem;
  margin-top: 8rem;
}
.delivered-imgs {
  display: flex;
}
.delivered-imgs img {
  border: 3px solid #fdf2e9;
  border-radius: 50%;
  height: 4.8rem;
  margin-right: -1.6rem;
  width: 4.8rem;
}
.delivered-imgs img:last-child {
  margin: 0;
}
.delivered-text {
  font-size: 1.8rem;
  font-weight: 600;
}

.delivered-text span {
  color: #cf711f;
  font-weight: 700;
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
  line-height: 1.6;
  margin: 0 0 4.8rem 0;
}

.btn:link,
.btn:visited {
  background-color: #e67e22;
  border-radius: 0.9rem;
  border: none;
  color: #fff;
  cursor: pointer;
  display: inline-block;
  font-size: 2rem;
  font-weight: 600;
  padding: 1.6rem 3.2rem;
  text-decoration: none;

  /* Put transition:  on original state; */
  transition: all 0.3s;
}
.btn-full:link,
.btn-full:visited {
  background-color: #e67e22;
  color: #fff;
}
.btn-full:hover,
.btn-full:active {
  background-color: #cf711f;
  color: #fff;
}

.btn--outline:link,
.btn--outline:visited {
  background-color: #fff;
  color: #333;
}
.btn--outline:hover,
.btn--outline:active {
  background-color: #fdf2e9;
  /* border: 3px solid #fff; */
  /* Trick to add border inside */
  box-shadow: inset 0 0 0 3px #fff;
}
.margin-right-sm {
  margin-right: 1.6rem;
}
</style>
