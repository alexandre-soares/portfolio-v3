<template>
  <v-container class="work">
    <h2 class="slide-in-bottom">
      Some of my work <span class="emojis">🖥</span>
    </h2>
    <p class="paragraph slide-in-bottom">
      Throughout the years I've been working with interesting clients & several
      exciting projects ideas, and here are some of them:
    </p>

    <Work-list />
  </v-container>
</template>

<script>
import WorkList from './work/WorkList.vue'
export default {
  components: { WorkList }
}
</script>

<style lang="scss" scoped>
.work {
  margin-bottom: 60px;
  z-index: 9999;
}
</style>
