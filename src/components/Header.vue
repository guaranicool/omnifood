<template>
  <header class="header">
    <img :src="imgLogo" alt="Omnifood logo" class="logo" />
    <Nav />
  </header>
</template>

<script>
import Nav from './Nav.vue';

export default {
  components: { Nav },

  data() {
    return {
      imgLogo: require('../assets/images/omnifood-logo.png'),
    };
  },
};
</script>

<style>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #fdf2e9;

  /* Because we want header to be sticky later */
  height: 9.6rem;
  padding: 0 4.8rem;
}

.logo {
  height: 2.2rem;
}
</style>
