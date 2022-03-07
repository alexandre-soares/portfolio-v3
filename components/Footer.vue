<template>
  <v-container class="footer">
    <h2 class="availability">
      <span class="green-circle pulse"></span>Available for
      <strong class="mx-1">remote</strong> positions
    </h2>
    <p>
      I’d be happy to hear from you if you are interested on my profile! Don't
      hesitate to contact me, I'll get back to you within 24 hours.
    </p>

    <div class="footer__actions">
      <Contact />
      <SocialMedias />
    </div>
  </v-container>
</template>

<script>
import SocialMedias from './SocialMedias.vue'
import Contact from './Contact.vue'
export default {
  name: 'Footer',
  components: { SocialMedias, Contact }
}
</script>

<style lang="scss" scoped>
.footer {
  padding-bottom: 80px !important;

  & p {
    @media only screen and (max-width: 479px) {
      text-align: center;
      width: 100%;
    }
  }

  &__actions {
    margin: 48px 0 0;
    display: flex;
    align-items: center;
    justify-content: space-between;

    @media only screen and (max-width: 768px) {
      flex-direction: column;
      gap: 32px;
    }
  }
}
</style>
