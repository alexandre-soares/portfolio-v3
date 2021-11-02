<template>
  <div class="grid-work">
    <!-- Laura's Portfolio -->
    <div
      class="card"
      :style="{
        'background-image':
          'url(' +
          require('@/static/img/portfolio/art-board-studio/laura-sibille-feature.png') +
          ')'
      }"
    >
      <span class="card__label">Front End Website</span>
      <h3 class="card__title">UX Designer - Portfolio</h3>
      <a
        href="https://www.laurasibille.com/"
        target="_blank"
        class="card__website ma-6"
        >Discover the project</a
      >
    </div>

    <!-- Requiem's Blog -->
    <div
      class="card"
      :style="{
        'background-image':
          'url(' +
          require('@/static/img/portfolio/art-board-studio/requiem-blog-featured-image.png') +
          ')'
      }"
    >
      <span class="card__label">Full Stack App</span>
      <h3 class="card__title">Requiem's Blog</h3>
      <a
        href="https://joker-s-blog.web.app/"
        target="_blank"
        class="card__website ma-6"
        >Discover the project</a
      >
      <a
        target="_blank"
        class="card__github ma-6"
        href="https://github.com/alexandre-soares/joker-blog"
        >Github</a
      >
    </div>

    <!-- Invoice App -->
    <div
      class="card"
      :style="{
        'background-image':
          'url(' +
          require('@/static/img/portfolio/art-board-studio/invoice-app-feature.png') +
          ')'
      }"
    >
      <span class="card__label">Full Stack App</span>
      <h3 class="card__title">Invoice App</h3>
      <a
        href="https://vuejs-invoice-app.web.app/"
        target="_blank"
        class="card__website ma-6"
        >Discover the project</a
      >
      <a
        target="_blank"
        class="card__github ma-6"
        href="https://github.com/alexandre-soares/vuejs-invoice-app"
        >Github</a
      >
    </div>

    <!-- Music Player -->
    <div
      class="card"
      :style="{
        'background-image':
          'url(' +
          require('@/static/img/portfolio/art-board-studio/music-player-feature.png') +
          ')'
      }"
    >
      <span class="card__label">Front End App</span>
      <h3 class="card__title">Music Player</h3>
      <a
        href="https://elastic-euler-fa1143.netlify.app"
        target="_blank"
        class="card__website ma-6"
        >Discover the project</a
      >
      <a
        target="_blank"
        class="card__github ma-6"
        href="https://github.com/alexandre-soares/vuejs-music-app"
        >Github</a
      >
    </div>

    <!-- Weather App -->
    <div
      class="card"
      :style="{
        'background-image':
          'url(' +
          require('@/static/img/portfolio/art-board-studio/weather-app-feature.png') +
          ')'
      }"
    >
      <span class="card__label">Full Stack App</span>
      <h3 class="card__title">Weather App</h3>
      <a
        href="https://vuejs-weather-app-7dab4.web.app/"
        target="_blank"
        class="card__website ma-6"
        >Discover the project</a
      >
      <a
        target="_blank"
        class="card__github ma-6"
        href="https://github.com/alexandre-soares/vuejs-weather-app"
        >Github</a
      >
    </div>

    <!-- Netflix Movie Api -->
    <div class="card">
      <video autoplay muted loop class="card__video">
        <source
          src="@/static/img/portfolio/art-board-studio/netflix-feature.webm"
          type="video/webm"
        />
      </video>

      <span class="card__label">Front End App</span>
      <h3 class="card__title">Netflix Movie Api</h3>
      <a
        href="https://quirky-hugle-b33382.netlify.app"
        target="_blank"
        class="card__website ma-6"
        >Discover the project</a
      >
      <a
        target="_blank"
        class="card__github ma-6"
        href="https://github.com/alexandre-soares/netflix-movie-app-nuxtjs"
        >Github</a
      >
    </div>

    <!-- 
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
       -->
  </div>
</template>

<script>
import { v1 as uuidv4 } from 'uuid'

export default {
  name: 'WorkGrid',
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
          thumbnail: require('@/static/img/portfolio/music-player-feature.png')
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
  grid-template-columns: repeat(6, 1fr);

  @media only screen and (max-width: 768px) {
    display: flex;
    flex-direction: column;
  }
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
  position: relative;
  overflow: hidden;

  @media only screen and (max-width: 768px) {
    min-height: auto;
  }

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

  &__video {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    z-index: -1;
    transform: scale(1.1);

    @media only screen and (max-width: 768px) {
      transform: scale(1.5) translateY(-25px);
    }
  }

  &__label {
    display: inline-block;
    margin: 40px 0px 20px;
    padding: 4px 16px;
    border-radius: 100px;
    background-color: hsla(0, 0%, 100%, 0.5);
    font-size: 12px;
    line-height: 16px;
    letter-spacing: 0.5px;
    text-transform: uppercase;
  }

  &__title {
    margin: 20px auto;
    width: 89%;
    color: hsla(0, 0%, 100%, 0.97);
    font-size: 48px;
    line-height: 48px;
    font-weight: 800;
    text-align: center;
    text-shadow: 0 1px 3px rgb(0 0 0 / 10%), 1px 1px 2px rgb(0 0 0 / 6%);
  }

  &__website {
    display: inline-block;
    margin-top: 0px;
    margin-right: 16px;
    margin-bottom: 0px;
    padding: 8px 16px;
    border-radius: 100px;
    background-color: #fff;
    color: #000;
    font-size: 16px;
    line-height: 24px;
    cursor: pointer;
    display: inline-block;
  }

  &__github {
    display: inline-block;
    margin: 0 16px 0 0;
    padding: 8px 16px;
    border-radius: 100px;
    background-color: #fff;
    color: #000;
    font-size: 16px;
    line-height: 24px;
    cursor: pointer;
    display: inline-block;
  }
}
</style>
