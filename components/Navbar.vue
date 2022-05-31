<template>
  <v-container>
    <div class="navbar my-6">
      <div class="navbar__brand">

        <nuxt-img src="/alex.jpg" alt="pic" />
        <span
          >Alexandre SOARES, <br />
          Smiling since 1996 😎</span
        >
      </div>

      <LazyHydrate when-visible>
        <SocialMedias />
      </LazyHydrate>
    </div>
  </v-container>
</template>

<script>
import LazyHydrate from 'vue-lazy-hydration'
import SocialMedias from './SocialMedias.vue'
export default {
  name: 'Navbar',
  components: { SocialMedias, LazyHydrate },
  data() {
    return {
      isActive: false
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
    line-height: 30px;
    font-weight: 600;

    & img {
      height: 90px;
      width: 90px;
      border-radius: 50%;
      margin-right: 20px;
      object-fit: cover;
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
