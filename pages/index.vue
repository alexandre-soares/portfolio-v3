<template>
  <div id="luxy">
    <Loader v-if="false" />
    <div v-if="true">
      <Navbar />
      <Hero />
      <Work />
      <Skills />
      <About />
      <Footer />
    </div>
  </div>
</template>

<script>
import Skills from '@/components/Skills.vue'
import Hero from '@/components/Hero.vue'
import Navbar from '@/components/Navbar.vue'
import Work from '@/components/Work.vue'
import About from '@/components/About.vue'
import Footer from '@/components/Footer.vue'
import Loader from '@/components/Loader.vue'
export default {
  components: {
    Navbar,
    Hero,
    Work,
    Skills,
    About,
    Footer,
    Loader
  },
  scrollToTop: true,
  data() {
    return {
      isLoading: true
    }
  },
  mounted() {
    window.scrollTo(0, 0)
    setTimeout(() => {
      this.isLoading = false
    }, 3000)
  }
}
</script>

<style></style>
