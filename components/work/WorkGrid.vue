<template>
  <div class="grid-work">
    <!-- Laura's Portfolio -->
    <div
      class="card"
      data-aos="slide-up"
      data-aos-offset="300"
      data-aos-delay="0"
      data-aos-duration="1700"
    >
      <span class="card__label">Front End Website</span>

      <h3 class="card__title">UX Designer - Portfolio</h3>
      <a
        href="https://www.laurasibille.com/"
        target="_blank"
        class="card__website ma-6"
        >Discover the project</a
      >

      <div class="card__skills">
        <BaseIcon
          :prettier-name="'NuxtJs'"
          :name-value="'nuxtjs.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />

        <BaseIcon
          :prettier-name="'Sass'"
          :name-value="'sass.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />
      </div>
    </div>

    <!-- Requiem's Blog -->
    <div
      class="card"
      data-aos="slide-up"
      data-aos-offset="300"
      data-aos-delay="200"
      data-aos-duration="1700"
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
        >Find the Github here</a
      >

      <div class="card__skills">
        <BaseIcon
          :prettier-name="'VueJs'"
          :name-value="'vuejs.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />

        <BaseIcon
          :prettier-name="'Firebase'"
          :name-value="'firebase.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />
      </div>
    </div>

    <!-- Invoice App -->
    <div
      class="card"
      data-aos="slide-up"
      data-aos-offset="300"
      data-aos-delay="0"
      data-aos-duration="1700"
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
        >Find the Github here</a
      >

      <div class="card__skills">
        <BaseIcon
          :prettier-name="'VueJs'"
          :name-value="'vuejs.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />

        <BaseIcon
          :prettier-name="'Firebase'"
          :name-value="'firebase.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />
      </div>
    </div>

    <!-- Music Player -->
    <div
      class="card"
      data-aos="slide-up"
      data-aos-offset="300"
      data-aos-delay="200"
      data-aos-duration="1700"
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
        >Find the Github here</a
      >

      <div class="card__skills">
        <BaseIcon
          :prettier-name="'VueJs'"
          :name-value="'vuejs.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />
      </div>
    </div>

    <!-- Weather App -->
    <div
      class="card"
      data-aos="slide-up"
      data-aos-offset="300"
      data-aos-delay="400"
      data-aos-duration="1700"
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
        >Find the Github here</a
      >

      <div class="card__skills">
        <BaseIcon
          :prettier-name="'VueJs'"
          :name-value="'vuejs.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />

        <BaseIcon
          :prettier-name="'Firebase'"
          :name-value="'firebase.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />
      </div>
    </div>

    <!-- Netflix Movie Api -->
    <div
      class="card"
      data-aos="slide-up"
      data-aos-offset="300"
      data-aos-delay="0"
      data-aos-duration="1700"
    >
      <video autoplay muted loop class="card__video">
        <source
          src="@/static/img/portfolio/netflix-feature.webm"
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
        >Find the Github here</a
      >

      <div class="card__skills">
        <BaseIcon
          :prettier-name="'VueJs'"
          :name-value="'vuejs.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />

        <BaseIcon
          :prettier-name="'Firebase'"
          :name-value="'firebase.svg'"
          :direction="'top'"
          :height="40"
          :width="40"
          :ml="10"
          :mr="10"
        />
      </div>
    </div>
  </div>
</template>

<script>
import BaseIcon from '../icons/BaseIcon.vue'

export default {
  name: 'WorkGrid',
  components: { BaseIcon }
}
</script>

<style lang="scss" scoped>
.grid-work {
  display: grid;
  grid-column-gap: 24px;
  grid-row-gap: 24px;
  grid-template-columns: repeat(6, 1fr);

  @media only screen and (max-width: 900px) {
    display: flex;
    flex-direction: column;
  }
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
    min-height: 350px;
  }

  @media only screen and (max-width: 479px) {
    height: 400px;
  }

  &:nth-child(1) {
    grid-row: 1;
    grid-column: 1 / 4;
    background-image: url('@/static/img/portfolio/laura-sibille-feature.png');
  }

  &:nth-child(2) {
    grid-column: 4 / 7;
    grid-row: 1;
    background-image: url('@/static/img/portfolio/requiem-blog-featured-image.png');
  }

  &:nth-child(3) {
    grid-row: 2;
    grid-column: 1 / 3;
    background-image: url('@/static/img/portfolio/invoice-app-feature.png');
  }

  &:nth-child(4) {
    grid-row: 2;
    grid-column: 3 / 5;
    background-image: url('@/static/img/portfolio/music-player-feature.png');
  }

  &:nth-child(5) {
    grid-row: 2;
    grid-column: 5 / 7;
    background-image: url('@/static/img/portfolio/weather-app-feature.png');
  }

  &:nth-child(6) {
    min-height: 650px;
    grid-row: 3;
    grid-column: 1 / 7;

    @media only screen and (max-width: 992px) {
      min-height: 450px;
    }

    @media only screen and (max-width: 768px) {
      min-height: 350px;
    }


    @media only screen and (max-width: 479px) {
      min-height: 400px;
    }
  }

  &__video {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    z-index: -1;
    transform: scale(1.2) translateX(-20px);

    @media only screen and (max-width: 768px) {
      transform: scale(2) translateX(-10px) translateY(-25px);
    }

    @media only screen and (max-width: 479px) {
      transform: scale(2.8) translateX(-5px) translateY(-25px);
    }
  }

  &__skills {
    display: flex;
    align-items: center;
    position: absolute;
    bottom: 15px;
    left: 50%;
    transform: translateX(-50%);

    & img {
      margin: 0 10px !important;
    }
  }

  &__label {
    display: inline-block;
    margin: 40px 0px 5px;
    padding: 4px 24px;
    border-radius: 100px;
    background-color: hsla(0, 0%, 100%, 0.5);
    font-size: 12px;
    line-height: 16px;
    letter-spacing: 0.5px;
    text-transform: uppercase;
  }

  &__title {
    color: rgba(255, 255, 255, 0.97);
    margin: 20px auto;
    width: 89%;
    font-size: 48px;
    line-height: 48px;
    font-weight: 800;
    text-shadow: 0 1px 10px rgb(0 0 0 / 20%), 1px 1px 5px rgb(0 0 0 / 16%);

    @media only screen and (max-width: 768px) {
      font-size: 36px;
      line-height: 48px;
      font-weight: 800;
    }
  }
}

a {
  display: inline-block;
  margin: 0 16px 0;
  padding: 8px 20px;
  border-radius: 100px;
  background-color: #fff;
  color: #000 !important;
  font-size: 16px;
  line-height: 24px;
  transition: all 0.2s ease-in;

  &:hover {
    transform: translateY(-5px);
    background-color: #f0efef;
  }
}
</style>
