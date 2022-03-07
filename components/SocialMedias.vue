<template>
  <div class="d-flex align-items-center">
    <BaseIconLink
      :prettier-name="'Download my resume'"
      :filename="'download.png'"
      :link="'/CV Alexandre SOARES 2022.pdf'"
      :height="30"
      :width="30"
      :ml="20"
      :mr="20"
    />

    <BaseIconLink
      :prettier-name="'LinkedIn'"
      :filename="'linkedin.svg'"
      :link="'https://www.linkedin.com/in/alex-ds-soares/'"
      :height="30"
      :width="30"
      :ml="20"
      :mr="20"
    />

    <BaseIconLink
      :prettier-name="'Github'"
      :filename="'github.svg'"
      :link="'https://github.com/alexandre-soares'"
      :height="30"
      :width="30"
      :ml="20"
      :mr="20"
    />
  </div>
</template>

<script>
import BaseIconLink from './icons/BaseIconLink.vue'
export default {
  name: 'SocialMedias',
  components: {
    BaseIconLink
  }
}
</script>

<style></style>
