<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import MainContent from './components/MainContent.vue'
import TestimonialSlider from './components/TestimonialSlider.vue';
import GetStarted from './components/GetStarted.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="wrapper">
    <Header />
    <Hero />
    <MainContent />
    <TestimonialSlider />
    <GetStarted />
    <Footer />
  </div>
</template>

<style scoped>
.wrapper {
  width: 100%;
  max-width: 1440px;
  min-height: 2639px;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
}

@media screen and (max-width: 1240px) {
  .wrapper {
    padding: 0 2.5rem;
    overflow: hidden;
  }
}

@media screen and (max-width: 980px) {
  .wrapper {
    padding: 0 2rem;
  }
}

@media screen and (max-width: 480px) {
  .wrapper {
    padding: 0 1rem;
  }
}

</style>
