<template>
  <div id="luxy">
    <Navbar />
    <Hero />
    <Work />
    <Skills />
    <About />
    <Footer />
  </div>
</template>

<script>
import Skills from '../components/Skills.vue'
import Hero from '../components/Hero.vue'
import Navbar from '../components/Navbar.vue'
import Work from '../components/Work.vue'
import About from '../components/About.vue'
import Footer from '../components/Footer.vue'
export default {
  components: {
    Navbar,
    Hero,
    Work,
    Skills,
    About,
    Footer
  },
  data() {
    return {
      isActive: false
    }
  }
}
</script>

<style></style>
