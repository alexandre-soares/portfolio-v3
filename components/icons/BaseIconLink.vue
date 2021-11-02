<template>
  <v-tooltip bottom>
    <template #activator="{ on, attrs }">
      <a :href="link" target="_blank">
        <img
          :src="'/img/icons/' + filename"
          alt="icon"
          v-bind="attrs"
          :style="{
            height: height + 'px',
            width: width + 'px',
            marginLeft: ml + 'px',
            marginRight: mr + 'px'
          }"
          v-on="on"
        />
      </a>
    </template>
    <span>{{ prettierName }} </span>
  </v-tooltip>
</template>

<script>
export default {
  name: 'BaseIconLink',
  props: ['filename', 'prettierName', 'link', 'height', 'width', 'ml', 'mr'],
  metaInfo() {
    return {
      filename() {
        return this.filename
      },
      prettierName() {
        return this.prettierName
      },
      link() {
        return this.link
      },
      height() {
        return this.height
      },
      width() {
        return this.width
      },
      ml() {
        return this.ml
      },
      mr() {
        return this.mr
      }
    }
  }
}
</script>

<style lang="scss" scoped>
img {
  cursor: pointer;
}
</style>
