<template>
  <v-container>
    <div class="navbar my-6">
      <div class="navbar__brand">
        <img src="@/static/alex-2.png" alt="pic" />
        <span
          >Alexandre SOARES, <br />
          Smiling since 1996 😎</span
        >
      </div>
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
  name: 'Navbar',
  methods: {
    darkMode() {
      this.$vuetify.theme.dark = !this.$vuetify.theme.dark
    }
  }
}
</script>

<style lang="scss" scoped>
.navbar {
  width: 100%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;

  @media only screen and (max-width: 500px) {
    flex-direction: column;
    justify-content: center;
    gap: 24px;
  }

  &__brand {
    display: flex;
    align-items: center;
    color: #000;
    font-size: 20px;
    line-height: 24px;
    font-weight: 600;

    & img {
      height: 90px;
      width: 90px;
      border-radius: 50%;
      margin-right: 20px;
    }
  }
}

.icon {
  margin-left: 20px;

  @media only screen and (max-width: 576px) {
    margin: 0 20px;
  }
}
</style>
