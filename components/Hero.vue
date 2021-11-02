<template>
  <v-container class="hero">
    <vue-typed-js
      :strings="strings"
      :loop="true"
      :type-speed="50"
      :back-speed="50"
      :bind-input-focus-events="true"
      :cursor-char="'|'"
      :back-delay="1000"
      :start-delay="1000"
    >
      <h1>
        Hi! I'm a VueJS Developer<br />
        but also <span class="typing"></span>
      </h1>
    </vue-typed-js>

    <a href="mailto:contact@alexandresoares.fr">
      <v-btn color="primary" large elevation="2" rounded class="mt-12 mb-1"
        >✉️ contact@alexandresoares.fr</v-btn
      >
    </a>

    <p>
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
        'a huge video games fan 🎮',
        'an optimiser freak 📦', 
        'a problem solver 💡!',
        'a cleaning addict 🧹!',
        'a gym rat 🏋️‍♂️',
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

  @media only screen and (max-width: 768px) {
    height: auto;
    align-items: center;
  }

  & h1 {
    height: auto;

    @media only screen and (max-width: 768px) {
      height: 50vh;
    }
  }

  & p {
    display: flex;
    align-items: center;

    @media only screen and (max-width: 768px) {
      justify-content: center;
    }
  }
}
</style>
