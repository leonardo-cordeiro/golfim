<template>
  <TheHeader />

  <TheIcons />

  <TheAbout />
</template>

<script setup>
import TheAbout from './components/TheAbout.vue'
import TheHeader from './components/TheHeader.vue'
import TheIcons from './components/TheIcons.vue'
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500&family=Raleway:wght@900&display=swap');

.text-raleway {
  font-family: 'Raleway', sans-serif;
}
.text-montserrat {
  font-family: 'Montserrat', sans-serif;
}

@for $i from 10 through 100 {
  .size-#{$i} {
    font-size: #{$i}px;
  }
}

html {
  font-size: 16px;
  scroll-behavior: smooth;

  @media (max-width: 720px) {
    font-size: 15px;
  }

  @media (max-width: 640px) {
    font-size: 14px;
  }

  @media (max-width: 560px) {
    font-size: 13px;
  }

  @media (max-width: 480px) {
    font-size: 12px;
  }

  @media (max-width: 400px) {
    font-size: 11px;
  }
}
</style>
