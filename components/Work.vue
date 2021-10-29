<template>
  <v-container class="work">
    <h2>Some of my work</h2>
    <p class="paragraph">
      Throughout the years I've been working with interesting clients & several
      exciting projects ideas, and here are some of them:
    </p>
    <div class="grid-work">
      <div
        v-for="project in projects"
        :key="project.id"
        class="card"
        :style="{ 'background-image': 'url(' + project.thumbnail + ')' }"
      >
        <span class="card__label">{{ project.type }}</span>
        <h3 class="card__title">{{ project.name }}</h3>
        <a target="_blank" class="card__website ma-6" :href="project.website"
          >Discover the project</a
        >
        <a
          v-if="project.github"
          target="_blank"
          class="card__github ma-6"
          :href="project.github"
          >Find the project on Github</a
        >
      </div>
    </div>
  </v-container>
</template>

<script>
import { v1 as uuidv4 } from 'uuid'
export default {
  data() {
    return {
      projects: [
        {
          id: uuidv4(),
          name: "Laura SIBILLE's Portfolio",
          skills: ['nuxtjs', 'sass'],
          type: 'Front End Website',
          website: 'https://www.laurasibille.com/',
          description: `
          This is the website I created for the UX-UI Designer Laura SIBILLE.
          `,
          thumbnail: require('@/static/img/portfolio/laura-sibille-feature.png')
        },
        {
          id: uuidv4(),
          name: `Requiem's Blog`,
          skills: ['vuejs', 'firebase', 'crud'],
          type: 'Full Stack App',
          website: 'https://joker-s-blog.web.app/',
          github: 'https://github.com/alexandre-soares/joker-blog',
          description: `
          A blog where you can find some interesting articles about video games.
          `,
          thumbnail: require('@/static/img/portfolio/requiem-blog-featured-image.png')
        },
        {
          id: uuidv4(),
          name: 'Netflix Movie Api',
          skills: ['vuejs', 'axios'],
          type: 'Front End App',
          website: 'https://quirky-hugle-b33382.netlify.app',
          github:
            'https://github.com/alexandre-soares/netflix-movie-app-nuxtjs',
          description: `
          A Netflix visual connected with a movie api to display a list of movies.
          `,
          thumbnail: require('@/static/img/portfolio/netflix-feature.png')
        },
        {
          id: uuidv4(),
          name: 'Invoice App',
          skills: ['vuejs', 'vuex', 'firebase'],
          type: 'Full Stack App',
          description: `
          An Invoice app with realtime update connected with Firebase.
          `,
          website: 'https://vuejs-invoice-app.web.app/',
          github: 'https://github.com/alexandre-soares/vuejs-invoice-app',
          thumbnail: require('@/static/img/portfolio/invoice-app-feature.png')
        },
        {
          id: uuidv4(),
          name: 'Music Player',
          skills: ['vuejs'],
          type: 'Front End App',
          website: 'https://elastic-euler-fa1143.netlify.app',
          github: 'https://github.com/alexandre-soares/vuejs-music-app',
          description: `
          A music player made with VueJS. Manipulation of audio files. (Desktop Only)
          `,
          thumbnail: require('@/static/img/portfolio/music-player-feature.png'),
          carouselImages: [
            require('@/static/img/portfolio/music-player-feature.png')
          ]
        },
        {
          id: uuidv4(),
          name: 'Weather App',
          skills: ['vuejs', 'firebase', 'crud'],
          type: 'Full Stack App',
          description: `
          An app where you can check the weather. The app is connected with Firebase.
          `,
          website: 'https://vuejs-weather-app-7dab4.web.app/',
          github: 'https://github.com/alexandre-soares/vuejs-weather-app',
          thumbnail: require('@/static/img/portfolio/weather-app-feature.png')
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.grid-work {
  display: grid;
  grid-column-gap: 24px;
  grid-row-gap: 24px;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
}

p {
  margin: 30px 0 40px;
}

.card {
  text-align: center;
  flex-direction: column;
  background-size: cover;
  background-position: center center;
  min-height: 600px;
  border-radius: 12px;

  &:nth-child(1) {
    grid-row: 1;
    grid-column: 1 / 4;
  }

  &:nth-child(2) {
    grid-column: 4 / 7;
    grid-row: 1;
  }

  &:nth-child(3) {
    grid-row: 2;
    grid-column: 1 / 3;
  }

  &:nth-child(4) {
    grid-row: 2;
    grid-column: 3 / 5;
  }

  &:nth-child(5) {
    grid-row: 2;
    grid-column: 5 / 7;
  }

  &:nth-child(6) {
    grid-row: 3;
    grid-column: 1 / 7;
  }

  &__label {
    display: inline-block;
    margin-top: 40px;
    margin-right: 0px;
    margin-left: 0px;
    padding: 4px 8px;
    justify-content: center;
    border-radius: 100px;
    background-color: hsla(0, 0%, 100%, 0.5);
    font-size: 12px;
    line-height: 16px;
    text-align: center;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    white-space: normal;
    object-fit: fill;
  }

  &__title {
    margin: 20px auto;
    width: 70%;
    color: hsla(0, 0%, 100%, 0.97);
    font-size: 48px;
    line-height: 48px;
    font-weight: 800;
    text-align: center;
    text-shadow: 0 1px 3px rgb(0 0 0 / 10%), 1px 1px 2px rgb(0 0 0 / 6%);
    object-fit: fill;
  }

  &__website {
    display: inline-block;
    margin-top: 0px;
    margin-right: 16px;
    margin-bottom: 0px;
    padding: 8px 16px;
    border: 2px solid #fff;
    border-radius: 100px;
    background-color: transparent;
    -webkit-transition: background-color 250ms ease, color 250ms ease;
    transition: background-color 250ms ease, color 250ms ease;
    color: #fff;
    font-size: 16px;
    line-height: 24px;
    text-align: center;
    cursor: pointer;
    display: inline-block;
  }

  &__github {
    display: inline-block;
    display: inline-block;
    margin-top: 0px;
    margin-right: 16px;
    margin-bottom: 0px;
    padding: 8px 16px;
    border: 2px solid #fff;
    border-radius: 100px;
    background-color: transparent;
    -webkit-transition: background-color 250ms ease, color 250ms ease;
    transition: background-color 250ms ease, color 250ms ease;
    color: #fff;
    font-size: 16px;
    line-height: 24px;
    text-align: center;
    cursor: pointer;
    display: inline-block;
  }
}
</style>
