<template>
  <section class="section-how">
    <div class="container">
      <span class="subheading">How it works</span>
      <h2 class="heading-secondary">
        Your daily dose of health in 3 simple steps
      </h2>
    </div>

    <!-- Grid container -->
    <div class="container">
      <div class="step-text-box"></div>

      <div class="step-img-box">
        <img :src="setpImgBoxA" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    setpImgBoxA: require('../assets/images/app/app-screen-1.png'),
  }),
};
</script>

<style></style>
