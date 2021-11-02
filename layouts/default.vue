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
h1 {
  margin-top: 0px;
  margin-bottom: 0px;
  font-family: 'Roboto', sans-serif;
  color: #000;
  font-size: 72px;
  line-height: 80px;
  font-weight: 600;

  @media only screen and (max-width: 768px) {
    font-size: 50px;
    line-height: 70px;
    font-weight: 400;
  }
}

h2 {
  font-family: 'Roboto', sans-serif;
  color: #000;
  font-size: 36px;
  line-height: 40px;
  font-weight: 700;

  @media only screen and (max-width: 768px) {
    font-size: 27px;
  }
}

p {
  width: 70%;
  margin-top: 12px;
  margin-right: 0px;
  margin-bottom: 0px;
  font-family: 'Roboto', sans-serif;
  color: #000;
  font-size: 24px;
  line-height: 48px;
  font-weight: 300;

  @media only screen and (max-width: 768px) {
    width: 90%;
    font-size: 20px;
    line-height: 36px;
  }
}

a {
  text-decoration: none;
}

.pointer {
  cursor: pointer;
}

.green-circle {
  height: 20px;
  width: 20px;
  background-color: #4cd264;
  border-radius: 50%;
  margin-right: 10px;
}

.icon {
  width: 30px;
  height: 30px;
  cursor: pointer;
}

button {
  text-transform: lowercase !important;
  font-family: 'Roboto', sans-serif !important;
  font-size: 16px !important;
}
</style>
