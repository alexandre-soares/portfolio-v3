<template>
  <footer class="footer">
    <v-container>
      <h2 class="d-flex align-center">
        <span class="green-circle"></span>Available for remote work
      </h2>
      <p>
        I’d be happy to hear from you if you are interested on my profile! Don't hesitate to contact me, I'll get back to you within 24 hours.
      </p>

      <v-row class="align-center justify-space-between mt-12">
        <a href="mailto:contact@alexandresoares.fr">
          <v-btn color="primary" large elevation="2" rounded
            >contact@alexandresoares.fr</v-btn
          >
        </a>
        <div>
          <v-tooltip bottom>
            <template #activator="{ on, attrs }">
              <a target="_blank" href="/CV Alexandre SOARES 2021.pdf">
                <img
                  src="static/img/icons/emailjs.svg"
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
              <img
                src="/img/icons/linkedin.svg"
                alt="icon"
                class="icon"
                v-bind="attrs"
                v-on="on"
              />
            </template>
            <span>Linkedin</span>
          </v-tooltip>
          <v-tooltip bottom>
            <template #activator="{ on, attrs }">
              <img
                src="/img/icons/github.svg"
                alt="icon"
                class="icon"
                v-bind="attrs"
                v-on="on"
              />
            </template>
            <span>Github</span>
          </v-tooltip>
        </div>
      </v-row>
    </v-container>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.footer {
  padding-bottom: 80px !important;
}
</style>
