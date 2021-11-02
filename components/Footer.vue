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
      <div class="d-flex align-items-center">
        <BaseIconLink
          :prettier-name="'Download my resume'"
          :filename="'download'"
          :type="'png'"
          :link="'/CV Alexandre SOARES 2021.pdf'"
          :height="30"
          :width="30"
          :ml="20"
          :mr="20"
        />

        <BaseIconLink
          :prettier-name="'LinkedIn'"
          :filename="'linkedin'"
          :type="'svg'"
          :link="'https://www.linkedin.com/in/alex-ds-soares/'"
          :height="30"
          :width="30"
          :ml="20"
          :mr="20"
        />

        <BaseIconLink
          :prettier-name="'Github'"
          :filename="'github'"
          :type="'svg'"
          :link="'https://github.com/alexandre-soares'"
          :height="30"
          :width="30"
          :ml="20"
          :mr="20"
        />
      </div>
    </div>
  </v-container>
</template>

<script>
import BaseIconLink from './icons/BaseIconLink.vue'
export default {
  name: 'Footer',
  components: { BaseIconLink }
}
</script>

<style lang="scss" scoped>
.footer {
  padding-bottom: 80px !important;

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
.icon {
  margin: 0 20px;
}

a {
  text-align: center;
  height: auto !important;
}
</style>
