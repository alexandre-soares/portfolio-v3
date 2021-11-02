<template>
  <div class="skills">
    <v-container>
      <h2>Ok great… but how can you help me ?</h2>

      <p class="paragraph">
        With my motivation to succeed, to help and to make things greater, I
        will find a way to help you!
      </p>

      <v-row class="cards">
        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'Javascript'"
              :name-value="'js.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'VueJs'"
              :name-value="'vuejs.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'NuxtJs'"
              :name-value="'nuxtjs.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Sass'"
              :name-value="'sass.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Vuetify'"
              :name-value="'vuetify.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Bootstrap'"
              :name-value="'bootstrap.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'TailwindCSS'"
              :name-value="'tailwindcss.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Building a custom responsive website</h3>
          <p class="card__paragraph">
            From product design to strategy, design systems, UX or UI. I solve
            complex problems through design, so you can achieve your business
            goals.
          </p>
        </div>

        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'NodeJs'"
              :name-value="'nodejs.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Firebase'"
              :name-value="'firebase.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Netlify'"
              :name-value="'netlify.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Server / Hosting</h3>
          <p class="card__paragraph">
            From product design to strategy, design systems, UX or UI. I solve
            complex problems through design, so you can achieve your business
            goals.
          </p>
        </div>

        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'GraphQL'"
              :name-value="'graphql.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Apollo GraphQL'"
              :name-value="'apollo-graphql.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Apis</h3>
          <p class="card__paragraph">
            From product design to strategy, design systems, UX or UI. I solve
            complex problems through design, so you can achieve your business
            goals.
          </p>
        </div>

        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'VS Code'"
              :name-value="'vscode.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Git'"
              :name-value="'git.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Jira'"
              :name-value="'jira.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Trello'"
              :name-value="'trello.svg'"
              :direction="'bottom'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Tools</h3>
          <p class="card__paragraph">
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
import BaseIcon from './icons/BaseIcon.vue'

export default {
  name: 'Skills',
  components: {
    BaseIcon
  }
}
</script>

<style lang="scss" scoped>
.skills {
  padding: 120px 0;
  background-color: black;
  color: #fff;

  display: flex;
  flex-direction: column;
  justify-content: center;

  @media only screen and (max-width: 768px) {
    padding: 60px 24px;
  }
}

.cards {
    display: flex;
    gap: 48px 96px;
    padding: 12px;
    margin-top: 30px;

    @media only screen and (max-width: 768px) {
      flex-direction: column;
      align-items: flex-start;
      gap: 24px;
    }
  }

 .card {
  &__title {
    margin: 16px 0;
    font-size: 20px;
    line-height: 28px;
    font-weight: 500;
  }

  &__paragraph {
    max-width: 400px;
    color: #a1a1a6 !important;
    font-size: 16px;
    line-height: 28px;
    font-weight: 300;
  }

  &__icons {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
 }
</style>
