<script setup lang="ts">
// import Intro from './sections/Intro.vue'
import Header from './sections/Header.vue'
import Hero from './sections/Hero.vue'
import About from './sections/About.vue'
import Gallery from './sections/Gallery.vue'
import Rooms from './sections/Rooms.vue'
import Footer from './sections/Footer.vue'
import Email from './sections/Email.vue'
import Maps from './sections/Maps.vue'
</script> 

<template>
  <div class="w-full h-screen grid
  grid-rows-[20vh_1fr]
  sm:grid-rows-[12vh_1fr]
  2xl:h-auto 2xl:grid-rows-[8vh_1fr]">
    <Header />

    <Hero />
  </div>

  <About />

  <Gallery />

  <Rooms />

  <Email />

  <Maps />

  <Footer />
</template> 

<style scoped></style> 
