<template>
  <div class="skills">
    <v-container>
      <h2>
        My weapons to make UX designs a reality <span class="emojis">⚔️</span>
      </h2>

      <p>
        With my motivation to succeed, to help and to make things greater, I
        will find a way to help you!
      </p>

      <v-row class="cards">
        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'VueJs'"
              :name-value="'vuejs.svg'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'NuxtJs'"
              :name-value="'nuxtjs.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Sass'"
              :name-value="'sass.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Vuetify'"
              :name-value="'vuetify.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Bootstrap'"
              :name-value="'bootstrap.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Front End Tools</h3>
          <p class="card__paragraph">
            Vue.js is a <strong>progressive JavaScript framework,</strong> which
            is used to <strong>build UIs (User Interfaces)</strong> and
            <strong>SPAs (Single-page Applications).</strong> With its
            <strong>component-based approach,</strong> the framework allows us
            to <strong>import</strong> components and
            <strong>reuse</strong> them wherever we need it. Combined with a
            <strong>powerful CSS framework</strong> like
            <strong>Vuetify</strong> or <strong>Bootstrap</strong>, developers
            are provided with all the tools they need to build
            <strong>rich and engaging user experiences.</strong>
          </p>
        </div>

        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'NodeJs'"
              :name-value="'nodejs.svg'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Firebase'"
              :name-value="'firebase.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Netlify'"
              :name-value="'netlify.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Heroku'"
              :name-value="'heroku.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Back End Tools / Hosting</h3>

          <p class="card__paragraph">
            Node.js is a <strong>fast, lightweight and efficient</strong> run
            time open source development platform used to
            <strong>build real-time, cross-platform, web applications.</strong>
            Combine this with the power of
            <strong>Netlify or Heroku </strong>and deploying/managing apps has
            never been that easy!
          </p>
        </div>

        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'GraphQL'"
              :name-value="'graphql.svg'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Apollo GraphQL'"
              :name-value="'apollo-graphql.svg'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Querying APIs / Third Party APIs</h3>
          <p class="card__paragraph">
            GraphQL is a <strong>query language</strong> for APIs and a runtime
            for <strong>fulfilling those queries</strong> with your existing
            data. GraphQL provides a
            <strong>complete and understandable</strong> description of the data
            in your API, gives clients the <strong>power to ask</strong> for
            exactly what <strong>they need.</strong>
            <strong>Third party APIs</strong> are APIs provided by third parties
            to allow you <strong>to access their functionality</strong> via
            JavaScript and use it on your site.
          </p>
        </div>

        <div class="card">
          <div class="card__icons">
            <BaseIcon
              :prettier-name="'VS Code'"
              :name-value="'vscode.svg'"
              :height="30"
              :width="30"
              :ml="0"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Git'"
              :name-value="'git.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Jira'"
              :name-value="'jira.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />

            <BaseIcon
              :prettier-name="'Trello'"
              :name-value="'trello.svg'"
              :height="30"
              :width="30"
              :ml="15"
              :mr="15"
            />
          </div>
          <h3 class="card__title">Development and Agile Tools</h3>
          <p class="card__paragraph">
            Web development is a <strong>continuous lifecycle</strong> involving
            multiple stages and iterations. Agile methodology
            <strong>increases performance</strong> and
            <strong>delivers valuable products</strong> by adapting to
            <strong>changing events</strong> in the workplace. They
            <strong>ensure a quick response </strong>to changes in every stage
            of production, including <strong>team communication,</strong>
            <strong>task management,</strong>
            <strong>issue tracking,</strong> and
            <strong>knowledge sharing.</strong> Those tools are designed to
            <strong>simplify and streamline</strong> the development lifecycle
            for web developers without compromising on performance.
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

  @media only screen and (max-width: 479px) {
    padding: 50px 16px;
  }
}

.cards {
  display: flex;
  gap: 48px 20px;
  padding: 12px;
  margin-top: 30px;

  @media only screen and (max-width: 768px) {
    flex-direction: column;
    align-items: flex-start;
    gap: 24px;
  }

  @media only screen and (max-width: 479px) {
    justify-content: center;
  }
}

.card {
  &__title {
    margin: 18px 0;
    font-size: 20px;
    line-height: 28px;
    font-weight: 500;
  }

  &__paragraph {
    width: 85%;
    max-width: 600px;
    margin: 0;
    color: #bdbdc0 !important;
    font-size: 16px;
    line-height: 28px;
    font-weight: 300;
    text-align: justify;

    @media only screen and (max-width: 479px) {
      width: 100%;
      max-width: none;
    }
  }

  &__icons {
    display: flex;
    align-items: center;
  }
}

strong {
  font-weight: bold;
}

p {
  width: 85%;
}
</style>
