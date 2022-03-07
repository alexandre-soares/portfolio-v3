<template>
  <v-app>
    <v-main>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {}
</script>

<style lang="scss">
body {
  background-color: #f5f8fa !important;
}

.theme--light.v-application {
  background-color: #f5f8fa !important;
  color: rgba(0, 0, 0, 0.87);
}

.v-application {
  font-family: 'Open Sans', sans-serif;
}

h1 {
  margin: 0;
  font-size: 72px;
  line-height: 80px;
  font-weight: 600;

  @media only screen and (max-width: 768px) {
    font-size: 40px;
    line-height: 50px;
  }
}

h2 {
  font-size: 36px;
  line-height: 40px;
  font-weight: 700;

  @media only screen and (max-width: 768px) {
    font-size: 27px;
  }
}

p {
  width: 70%;
  margin: 12px 0;
  font-size: 24px;
  line-height: 48px;
  font-weight: 300;

  @media only screen and (max-width: 768px) {
    width: 100%;
    font-size: 20px;
    line-height: 36px;
  }
}

a {
  text-decoration: none;
}

img {
  height: 100%;
  width: 100%;
}
// Emojis

.emojis {
  margin-left: 15px;
  margin-top: 4px;
}

// Container

.container {
  max-width: 1440px !important;
  padding-right: 100px !important;
  padding-left: 100px !important;

  @media only screen and (max-width: 1200px) {
    padding: 12px 48px !important;
  }

  @media only screen and (max-width: 768px) {
    padding: 12px 24px !important;
  }

  @media only screen and (max-width: 479px) {
    padding: 12px 16px !important;
  }
}

// Available for remote work

.availability {
  font-size: 16px;
  color: #000;
  font-weight: 500;
  display: flex;
  align-items: center;

  @media only screen and (max-width: 768px) {
    justify-content: center;
  }
}

.green-circle {
  height: 15px;
  width: 15px;
  background-color: #4cd264;
  border-radius: 50%;
  margin-right: 15px;
}

.pulse {
  background-color: 4cd264;
  border-radius: 50%;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0% {
    box-shadow: 0 0 0 2px #4cd264;
  }
  100% {
    box-shadow: 0 0 0 10px transparent;
  }
}

// Buttons

button {
  text-transform: lowercase !important;
  font-size: 16px !important;
  transition: all 0.3s ease-in;

  &:hover {
    transform: translateY(-5px);
  }
}
</style>
