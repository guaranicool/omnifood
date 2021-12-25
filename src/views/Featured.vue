<template>
  <section class="section-featured">
    <div class="container">
      <h2 class="heading-featured-in">As featured in</h2>
      <div class="logos">
        <img :src="techrunchImg" alt="Techrunch Logo" />
        <img :src="businessInsiderImg" alt="Business Insider Logo" />
        <img :src="theNYTImg" alt="The New York Times logo" />
        <img :src="forbesImg" alt="Forbes logo" />
        <img :src="usaTodayImg" alt="USA Today logo" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    techrunchImg: require('../assets/images/logos/techcrunch.png'),
    businessInsiderImg: require('../assets/images/logos/business-insider.png'),
    theNYTImg: require('../assets/images/logos/the-new-york-times.png'),
    forbesImg: require('../assets/images/logos/forbes.png'),
    usaTodayImg: require('../assets/images/logos/usa-today.png'),
  }),
};
</script>

<style>
.section-featured {
  padding: 4.8rem 0 3.2rem 0;
}
.heading-featured-in {
  color: #888;
  font-size: 1.4rem;
  font-weight: 500;
  letter-spacing: 0.75px;
  text-align: center;
  text-transform: uppercase;
  margin-bottom: 2.4rem;
}
.logos {
  display: flex;
  justify-content: space-around;
}
.logos img {
  height: 3.2rem;
  filter: brightness(0);
  opacity: 50%;
}
</style>
