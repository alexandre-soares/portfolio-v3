<template>
  <v-container class="work">
    <h2>Some of my work</h2>
    <p class="paragraph">
      Throughout the years I've been working with interesting clients & several
      exciting projects ideas, and here are some of them:
    </p>
    <Work-grid />
  </v-container>
</template>

<script>
import WorkGrid from './work/WorkGrid.vue'
export default {
  components: { WorkGrid },
}
</script>

<style lang="scss" scoped></style>
