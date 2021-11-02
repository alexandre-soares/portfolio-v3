<template>
  <v-container>
    <div class="navbar my-6">
      <div class="navbar__brand">
        <v-lazy
          v-model="isActive"
          :options="{
            threshold: 0.5
          }"
          transition="fade-transition"
        >
          <img src="@/static/alex-2.png" alt="pic" />
        </v-lazy>

        <v-lazy
          v-model="isActive"
          :options="{
            threshold: 0.5
          }"
          transition="fade-transition"
        >
          <span
            >Alexandre SOARES, <br />
            Smiling since 1996 😎</span
          >
        </v-lazy>
      </div>

      <v-lazy
        v-model="isActive"
        :options="{
          threshold: 0.5
        }"
        transition="fade-transition"
      >
        <SocialMedias />
      </v-lazy>
    </div>
  </v-container>
</template>

<script>
import SocialMedias from './SocialMedias.vue'
export default {
  name: 'Navbar',
  components: { SocialMedias },
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
