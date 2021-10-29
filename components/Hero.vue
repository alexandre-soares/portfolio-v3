<template>
  <v-container class="hero">
    <vue-typed-js :strings="strings" :loop="true" :show-cursor="false">
      <h1>
        Hi! I'm a Front End Developer<br />
        but also <span class="typing"></span>
      </h1>
    </vue-typed-js>
    <v-chip color="primary" class="mt-6 mb-3 pointer"
      >contact@alexandresoares.fr</v-chip
    >
    <p class="d-flex align-center">
      <span class="green-circle"></span>
      Looking for remote works
    </p>
  </v-container>
</template>

<script>
import { VueTypedJs } from 'vue-typed-js'
export default {
  components: {
    VueTypedJs
  },
  data() {
    return {
      strings: [
        'a huge fan of games 🎮!',
        'a cleaning addict!',
        'a problem solver 🤔!'
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.hero {
  height: 70vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}
</style>
