<template>
  <div id="luxy">
    <Navbar />
    <Hero />
    <Work />
    <About />
  </div>
</template>

<script>
import About from '../components/About.vue'
import Hero from '../components/Hero.vue'
import Navbar from '../components/Navbar.vue'
import Work from '../components/Work.vue'
export default {
  components: {
    Navbar,
    Hero,
    Work,
    About
  }
}
</script>

<style></style>
