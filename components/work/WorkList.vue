<template>
  <div v-if="show" class="work-list">
    <div
      v-for="(project, i) in projects"
      :key="i"
      class="card"
      data-aos="slide-up"
      data-aos-offset="300"
      data-aos-delay="0"
      data-aos-duration="1700"
    >
      <a :href="project.link" target="_blank">
        <div class="card__image">
          <div class="card__image--overlay">Discover the project</div>

          <video
            v-if="!isSafari && project.video"
            autoplay
            muted
            loop
            playsInline
            controls
            :src="`/img/portfolio/${project.video}`"
            type="video/mp4"
            class="card__video"
          >
            <!-- fallback -->
            <p>Your browser does not support HTML5 video.</p>
          </video>

          <img
            v-else
            :src="`/img/portfolio/${project.image}`"
            :alt="project.title"
          />
        </div>
      </a>

      <div class="card__infos">
        <span class="card__type">{{ project.type }}</span>

        <h3 class="card__title">{{ project.title }}</h3>

        <p class="card__description">{{ project.description }}</p>
        <div class="card__skills">
          <span class="card__label card__label--title">Used Tools:</span>
          <div class="card__icons">
            <BaseIcon
              v-for="(skill, index) in project.usedTools"
              :key="index"
              :prettier-name="skill | capitalize"
              :name-value="`${skill}.svg`"
              :direction="'top'"
              :height="40"
              :width="40"
              :ml="10"
              :mr="10"
            />
          </div>
        </div>

        <div class="card__skills">
          <span class="card__label card__label--title">Learned Skills:</span>
          <div class="card__tools">
            <span
              v-for="(skill, index) in project.learnedSkills"
              :key="index"
              class="card__label"
            >
              {{ skill }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BaseIcon from '../icons/BaseIcon.vue'

export default {
  name: 'WorkList',
  components: { BaseIcon },
  filters: {
    capitalize(value) {
      if (!value) return ''
      value = value.toString()
      return value.charAt(0).toUpperCase() + value.slice(1)
    }
  },
  data() {
    return {
      isSafari: false,
      show: false,
      projects: [
        {
          title: 'UX Designer - Portfolio',
          type: 'Front End Website',
          link: 'https://www.laurasibille.com/',
          description: 'A Portfolio for a UX Designer',
          image: 'laura-sibille-feature.png',
          usedTools: ['nuxtjs', 'sass'],
          learnedSkills: ['Client Relation', 'Wireframe Coding']
        },
        {
          title: `Requiem's Blog`,
          type: 'Full Stack App',
          link: 'https://joker-s-blog.web.app/',
          description: 'A blog where you can see posts about video games',
          image: 'requiem-blog-featured.png',
          usedTools: ['VueJS', 'Firebase'],
          learnedSkills: ['CRUD', 'REST API']
        },
        {
          title: 'Invoice App',
          type: 'Full Stack App',
          link: 'https://vuejs-invoice-app.web.app/',
          description:
            'A invoice app where you can easily create, modify or delete invoices',
          image: 'invoice-app-feature.png',
          github: '',
          usedTools: ['VueJS', 'Firebase'],
          learnedSkills: ['CRUD', 'REST API']
        },
        {
          title: 'Music Player App',
          type: 'Front End App',
          link: 'https://elastic-euler-fa1143.netlify.app',
          description: 'A Music Player application',
          image: 'music-player-feature.png',
          github: '',
          usedTools: ['VueJS'],
          learnedSkills: ['File Gestion']
        },
        {
          title: 'Weather App',
          type: 'Full Stack App',
          link: 'https://vuejs-weather-app-7dab4.web.app/',
          description:
            'A basic wheater app displaying weather informations for a choosen city',
          image: 'weather-app-feature.png',
          github: '',
          usedTools: ['VueJS'],
          learnedSkills: ['REST API']
        },
        {
          title: 'Netflix Movie Api',
          type: 'Front End App',
          link: 'https://quirky-hugle-b33382.netlify.app',
          description:
            'A "Netflix style" app where you can access to movie informations',
          image: 'netflix-feature.png',
          usedTools: ['VueJS'],
          learnedSkills: ['REST API'],
          video: 'netflix-feature.mp4'
        }
      ]
    }
  },
  mounted() {
    // Test if browser is safari
    this.isSafari = /^((?!chrome|android).)*safari/i.test(navigator.userAgent)

    // Hide list when loaded
    this.show = true
  }
}
</script>

<style lang="scss" scoped>
.work-list {
  display: flex;
  gap: 24px;
  flex-direction: column;
}

.card {
  text-align: center;
  display: flex;
  gap: 32px;
  align-items: flex-start;
  justify-content: flex-start;
  padding: 24px;

  @media only screen and (max-width: 768px) {
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  &__image {
    border-radius: 12px;
    overflow: hidden;
    min-width: 350px;
    max-width: 450px;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    position: relative;

    & img {
      object-fit: cover;
    }

    &--overlay {
      display: none !important;
      position: absolute;
      top: 0;
      left: 0;
      color: white;
      background-color: rgba(0, 0, 0, 0.363);
      z-index: 9999;
      height: 100%;
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
    }

    video {
      border-radius: 15px;
      height: 100%;
      width: 100%;
      transform: scale(1.3) translateX(-5px);
    }

    &:hover .card__image--overlay {
      display: flex !important;
    }
  }

  &__infos {
    text-align: left;

    @media only screen and (max-width: 768px) {
      min-width: 350px;
      max-width: 450px;
    }
  }

  &__skills {
    display: flex;
    gap: 10px;
    align-items: center;
    bottom: 15px;
    margin: 32px 0;

    @media only screen and (max-width: 768px) {
      flex-direction: column;
    }
  }

  &__icons,
  &__tools {
    display: flex;
    gap: 10px;
    @media only screen and (max-width: 768px) {
      display: flex;
    }
  }

  &__label,
  &__type {
    padding: 4px 24px;
    border-radius: 100px;
    background-color: white;
    font-size: 12px;
    line-height: 16px;
    letter-spacing: 0.5px;
    text-transform: uppercase;

    @media only screen and (max-width: 768px) {
      padding: 4px 12px;
    }

    &--title {
      background-color: transparent;
      padding-left: 0;

      @media only screen and (max-width: 768px) {
        padding-right: 4px;
      }
    }
  }

  &__type {
    @media only screen and (max-width: 768px) {
      display: block;
      max-width: 200px;
      margin: 0 auto;
      text-align: center;
    }
  }

  &__title {
    color: rgba(49, 49, 49, 0.97);
    margin: 20px auto;
    font-size: 48px;
    line-height: 48px;
    font-weight: 800;

    @media only screen and (max-width: 768px) {
      font-size: 36px;
      line-height: 48px;
      font-weight: 800;
    }
  }
}

p {
  width: 100%;
}
</style>
