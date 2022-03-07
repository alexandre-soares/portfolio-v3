<template>
  <v-tooltip top>
    <template #activator="{ on, attrs }">
      <img
        :src="'/img/icons/' + nameValue"
        :alt="`${prettierName} icon`"
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
  props: {
    nameValue: {
      type: String,
      default: null
    },
    prettierName: {
      type: String,
      default: null
    },
    height: {
      type: Number,
      default: null
    },
    width: {
      type: Number,
      default: null
    },
    ml: {
      type: Number,
      default: null
    },
    mr: {
      type: Number,
      default: null
    }
  }
}
</script>

<style lang="scss" scoped>
img {
  cursor: help;
}

img[alt='Copy to clipboard icon'] {
  cursor: pointer;
}
</style>
