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
        <div class="d-flex align-items-center">
          <BaseIconLink
            :prettier-name="'Download my resume'"
            :filename="'download'"
            :type="'png'"
            :link="'/CV Alexandre SOARES 2021.pdf'"
            :height="30"
            :width="30"
            :ml="20"
            :mr="20"
          />

          <BaseIconLink
            :prettier-name="'LinkedIn'"
            :filename="'linkedin'"
            :type="'svg'"
            :link="'https://www.linkedin.com/in/alex-ds-soares/'"
            :height="30"
            :width="30"
            :ml="20"
            :mr="20"
          />

          <BaseIconLink
            :prettier-name="'Github'"
            :filename="'github'"
            :type="'svg'"
            :link="'https://github.com/alexandre-soares'"
            :height="30"
            :width="30"
            :ml="20"
            :mr="0"
          />
        </div>
      </v-lazy>
    </div>
  </v-container>
</template>

<script>
import BaseIconLink from './icons/BaseIconLink.vue'
export default {
  name: 'Navbar',
  components: { BaseIconLink },
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
    line-height: 24px;
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
