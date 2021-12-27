<template>
  <main>
    <Header />
    <Hero />
    <Featured />
    <How />
  </main>

  <router-view />
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Featured from './views/Featured.vue';
import How from './views/How.vue';

export default {
  name: 'App',
  components: { Header, Hero, Featured, How },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;600;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  /* font-size: 10px; */

  /* 10px / 16px = 0.625 = 62.5% */
  /* Percentage of user's browser font-size setting */
  /* 10px = 1rem */
  font-size: 62.5%;
  overflow-x: hidden;
}

body {
  font-family: 'Rubik', sans-serif;
  line-height: 1;
  font-weight: 400;
  color: #555;

  /* Only works if there is nothing absolutely positioned in relation to body */
  overflow-x: hidden;
}
.container {
  max-width: 120rem;
  padding: 0 3.2rem;
  margin: 0 auto;
}
.grid {
  display: grid;
  column-gap: 6.4rem;
  row-gap: 9.6rem;
  align-items: center;
}
.grid--2--cols {
  grid-template-columns: repeat(2, 1fr);
}

.heading-primary,
.heading-secondary,
.heading-tertiary {
  font-weight: 700;
  color: #333;
  /* color: #45260a; */
  /* color: #343a40; */
  letter-spacing: -0.5px;
}

.heading-primary {
  font-size: 5.2rem;
  line-height: 1.05;
  margin-bottom: 3.2rem;
}

.heading-secondary {
  font-size: 4.4rem;
  line-height: 1.2;
  margin-bottom: 9.6rem;
}

.heading-tertiary {
  font-size: 3rem;
  line-height: 1.2;
  margin-bottom: 3.2rem;
}

.subheading {
  display: block;
  font-size: 1.6rem;
  font-weight: 500;
  color: #cf711f;
  text-transform: uppercase;
  margin-bottom: 1.6rem;
  letter-spacing: 0.75px;
}
</style>
