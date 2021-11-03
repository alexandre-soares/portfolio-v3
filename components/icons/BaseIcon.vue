<template>
  <v-tooltip top>
    <template #activator="{ on, attrs }">
      <img
        :src="'/img/icons/' + nameValue"
        alt="icon"
        :style="{
          height: height + 'px',
          width: width + 'px',
          marginLeft: ml + 'px',
          marginRight: mr + 'px'
        }"
        v-bind="attrs"
        class="icon"
        v-on="on"
      />
    </template>
    <span>{{ prettierName }}</span>
  </v-tooltip>
</template>

<script>
export default {
  name: 'BaseIcon',
  props: [
    'nameValue',
    'prettierName',
    'height',
    'width',
    'ml',
    'mr'
  ],
  metaInfo() {
    return {
      nameValue() {
        return this.nameValue
      },
      prettierName() {
        return this.prettierName
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
  cursor: help;
}
</style>
