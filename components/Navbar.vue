<template>
  <v-container>
    <v-row class="justify-space-between my-6">
      <div>
        <span>Alexandre <strong>SOARES</strong></span>
      </div>
      <div>
        <v-tooltip bottom>
          <template #activator="{ on, attrs }">
            <a target="_blank" href="/CV Alexandre SOARES 2021.pdf">
              <img
                src="static/img/icons/emailjs.svg"
                alt="icon"
                class="about__icon"
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
              class="about__icon"
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
              class="about__icon"
              v-bind="attrs"
              v-on="on"
            />
          </template>
          <span>Github</span>
        </v-tooltip>
      </div>
    </v-row>
  </v-container>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
img {
  width: 30px;
  height: 30px;
  cursor: pointer;
  margin-left: 20px;
}
</style>
