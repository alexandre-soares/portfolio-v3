<template>
  <v-container class="about">
    <h2>Who am I?</h2>
    <p>
      Hi again! I am Alexandre Soares, Portuguese Front End developer born &
      raised in Lyon, France, but currently living in Bulgaria for the past 3
      years.
    </p>
    <p>
      I studied IT at Uni for 3 years but having still physics lessons didn’t
      convince me to pursue this way 🤷‍♂️ so I changed for 100% coding education.
      Since 2018 I’m working with VueJS & NuxtJs between blows of vacuum
      cleaner.
    </p>
    <p>
      I feel relieved when things are structured and optimized in every aspects
      of my life - especially at work - but I swear I am not a robot (at least I
      pass the captcha on websites 🤖)! I think my coach secretly tries to kill
      me everyday at the gym but still obviously failing 😁
    </p>
  </v-container>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.about {
  margin: 120px auto;

  @media only screen and (max-width: 768px) {
    margin: 60px auto;
  }
}
</style>
