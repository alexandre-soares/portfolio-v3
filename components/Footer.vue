<template>
  <v-container class="footer">
    <h2 class="availability">
      <span class="green-circle"></span>Available for remote positions
    </h2>
    <p>
      I’d be happy to hear from you if you are interested on my profile! Don't
      hesitate to contact me, I'll get back to you within 24 hours.
    </p>

    <div class="footer__actions">
      <a href="mailto:contact@alexandresoares.fr">
        <v-btn color="primary" large elevation="2" rounded
          >✉️ contact@alexandresoares.fr</v-btn
        >
      </a>

      <SocialMedias />
    </div>
  </v-container>
</template>

<script>
import SocialMedias from './SocialMedias.vue'
export default {
  name: 'Footer',
  components: { SocialMedias }
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
