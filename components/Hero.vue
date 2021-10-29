<template>
  <v-container class="hero">
    <vue-typed-js :strings="strings" :loop="true" :show-cursor="false">
      <h1>
        Hi! I'm a Front End Developer<br />
        but also <span class="typing"></span>
      </h1>
    </vue-typed-js>
    <a href="mailto:contact@alexandresoares.fr">
      <v-btn color="primary" large elevation="2" rounded
        >contact@alexandresoares.fr</v-btn
      >
    </a>
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
