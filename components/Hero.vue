<template>
  <v-container class="hero slide-in-bottom">
    <h1>Hi! I'm a VueJS Developer!</h1>

    <Contact />

    <p class="availability">
      <span class="green-circle pulse"></span>
      Looking for <strong class="mx-1">remote</strong> positions
    </p>
  </v-container>
</template>

<script>
import Contact from './Contact.vue'
export default {
  name: 'Hero',
  components: { Contact }
}
</script>

<style lang="scss" scoped>
.hero {
  height: 65vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;

  @media only screen and (max-width: 768px) {
    height: auto;
    align-items: center;
  }

  &__btn {
    margin: 24px 0;
  }
}

h1 {
  padding: 32px 0;
}
</style>
