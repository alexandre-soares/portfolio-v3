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
.v-application {
  font-family: 'Open Sans', sans-serif;
}

h1 {
  margin: 0;
  font-size: 72px;
  line-height: 80px;
  font-weight: 600;

  @media only screen and (max-width: 768px) {
    font-size: 48px;
    line-height: 70px;
    font-weight: 400;
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
    width: 90%;
    font-size: 20px;
    line-height: 36px;
  }
}

a {
  text-decoration: none;
}

.container {
  max-width: 1440px;
  padding-right: 100px;
  padding-left: 100px;

  @media only screen and (max-width: 1200px) {
    padding: 12px 48px;
  }

  @media only screen and (max-width: 768px) {
    padding: 12px 24px;
  }
}

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
  margin-right: 10px;
}

// BUTTONS

button {
  text-transform: lowercase !important;
  font-size: 16px !important;
  transition: all 0.3s ease-in;

  &:hover {
    transform: translateY(-5px);
  }
}
</style>
