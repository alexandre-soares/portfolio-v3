<template>
  <div class="about">
    <v-container>
      <h2>Ok great… but how can you help me ?</h2>
      <p class="paragraph">
        With my motivation to succeed, to help and to make things greater, I
        will find a way to help you!
      </p>

      <v-row class="about__cards">
        <div class="about__card">
          <div class="icons">
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/js.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Javscript</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/vuejs.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>VueJs</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/nuxtjs.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>NuxtJs</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/sass.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Sass</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/vuetify.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Vuetify</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/bootstrap.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Bootstrap</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/tailwindcss.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>TailwindCSS</span>
            </v-tooltip>
          </div>
          <h3 class="about__title">Building a custom responsive website</h3>
          <p class="about__paragraph">
            From product design to strategy, design systems, UX or UI. I solve
            complex problems through design, so you can achieve your business
            goals.
          </p>
        </div>

        <div class="about__card">
          <div class="icons">
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/nodejs.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>NodeJs</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/netlify.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Netlify</span>
            </v-tooltip>
          </div>
          <h3 class="about__title">Server / Hosting</h3>
          <p class="about__paragraph">
            From product design to strategy, design systems, UX or UI. I solve
            complex problems through design, so you can achieve your business
            goals.
          </p>
        </div>

        <div class="about__card">
          <div class="icons">
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/graphql.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>GraphQL</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/apollo-graphql.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Apollo GraphQL</span>
            </v-tooltip>
          </div>
          <h3 class="about__title">Apis</h3>
          <p class="about__paragraph">
            From product design to strategy, design systems, UX or UI. I solve
            complex problems through design, so you can achieve your business
            goals.
          </p>
        </div>

        <div class="about__card">
          <div class="icons">
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/vscode.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Visual Studio Code</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/git.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Git</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/jira.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Jira</span>
            </v-tooltip>
            <v-tooltip bottom>
              <template #activator="{ on, attrs }">
                <img
                  src="/img/icons/trello.svg"
                  alt="icon"
                  class="icon"
                  v-bind="attrs"
                  v-on="on"
                />
              </template>
              <span>Trello</span>
            </v-tooltip>
          </div>
          <h3 class="about__title">Tools</h3>
          <p class="about__paragraph">
            From product design to strategy, design systems, UX or UI. I solve
            complex problems through design, so you can achieve your business
            goals.
          </p>
        </div>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.about {
  padding-top: 120px;
  padding-bottom: 120px;
  background-color: black;
  color: white !important;
  display: flex;
  flex-direction: column;
  justify-content: center;

  &__cards {
    display: flex;
    flex-direction: row;
    gap: 64px;
    padding: 12px;
    margin-top: 30px;
  }

  & h2 {
    font-family: 'Roboto', sans-serif;
    color: #fff;
    font-size: 36px;
    line-height: 40px;
    font-weight: 700;
  }

  &__title {
    width: 100%;
    max-width: 400px;
    margin-top: 16px;
    margin-bottom: 0px;
    color: #fff;
    font-size: 20px;
    line-height: 28px;
    font-weight: 500;
  }

  & p {
    color: #fff;
    margin-bottom: 32px;
  }

  &__paragraph {
    max-width: 400px;
    margin-top: 4px;
    margin-bottom: 0px;
    color: #a1a1a6 !important;
    font-size: 16px;
    line-height: 24px;
    font-weight: 300;
  }

  &icons {
    margin-bottom: 10px;
  }

  &icon {
    height: 30px;
    width: 30px;
    margin-right: 10px;
  }
}
</style>
