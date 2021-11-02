<template>
  <v-container class="footer">
    <h2 class="availability">
      <span class="green-circle"></span>Available for remote work
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
        <v-tooltip bottom>
          <template #activator="{ on, attrs }">
            <a
              target="_blank"
              class="download"
              href="/CV Alexandre SOARES 2021.pdf"
            >
              <img
                src="@/static/img/icons/download.png"
                alt="icon"
                class="icon"
                v-bind="attrs"
                v-on="on"
              />
            </a>
          </template>
          <span>Download my resume</span>
        </v-tooltip>
        <v-tooltip bottom>
          <template #activator="{ on, attrs }">
            <a
              href="https://www.linkedin.com/in/alex-ds-soares/"
              target="_blank"
            >
              <img
                src="/img/icons/linkedin.svg"
                alt="icon"
                class="icon"
                v-bind="attrs"
                v-on="on"
              />
            </a>
          </template>
          <span>Linkedin</span>
        </v-tooltip>
        <v-tooltip bottom>
          <template #activator="{ on, attrs }">
            <a href="https://github.com/alexandre-soares" target="_blank">
              <img
                src="/img/icons/github.svg"
                alt="icon"
                class="icon"
                v-bind="attrs"
                v-on="on"
              />
            </a>
          </template>
          <span>Github</span>
        </v-tooltip>
      </div>
    </div>
  </v-container>
</template>

<script>
export default {
  name: 'Footer',
  methods: {
    darkMode() {
      this.$vuetify.theme.dark = !this.$vuetify.theme.dark
    }
  }
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
