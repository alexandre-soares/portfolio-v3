<template>
  <div class="contact">
    <a href="mailto:contact@alexandresoares.fr">
      <v-btn color="primary" large elevation="2" rounded
        >✉️ contact@alexandresoares.fr</v-btn
      >
    </a>

    <div class="copy" @click="copyToClipboard()">
      <BaseIcon
        :prettier-name="'Copy to clipboard'"
        :name-value="'copy.svg'"
        :height="35"
        :width="35"
        :ml="20"
        :mr="10"
      />
      <span v-if="showSuccessMessage" class="alert alert--success"
        >Copied to clipboard!</span
      >
      <span v-if="showErrorMessage" class="alert alert--error"
        >Something went wrong!</span
      >
    </div>
  </div>
</template>

<script>
import BaseIcon from './icons/BaseIcon.vue'

export default {
  name: 'Contact',
  components: { BaseIcon },
  data() {
    return {
      showSuccessMessage: false,
      showErrorMessage: false
    }
  },
  methods: {
    copyToClipboard() {
      try {
        navigator.clipboard.writeText('contact@alexandresoares.fr')
        this.showSuccessMessage = true

        setTimeout(() => {
          this.showSuccessMessage = false
        }, 5000)
      } catch (error) {
        this.showSuccessMessage = false
        this.showErrorMessage = true

        setTimeout(() => {
          this.showErrorMessage = false
        }, 5000)
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.contact,
.copy {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.alert {
  padding: 10px;
  margin-left: 5px;
  border: 1px solid transparent;
  border-radius: 8px;

  &--success {
    color: #3c763d;
    background-color: #dff0d8;
    border-color: #d6e9c6;
  }

  &--error {
    color: #a94442;
    background-color: #f2dede;
    border-color: #ebccd1;
  }
}
</style>
