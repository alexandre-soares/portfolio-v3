<template>
  <v-container class="about">
    <h2>Who am I?<span class="emojis">😈</span></h2>
    <p>
      Hi again! I am Alexandre Soares, a portuguese
      <strong>Front End developer</strong> born & raised in Lyon, France, but
      currently <strong>living in Bulgaria</strong> for the past 3 years.
    </p>
    <p>
      I studied IT at University for 3 years but having still chemistry lessons
      didn’t convince me to pursue this way 🤷‍♂️ so I changed for 100% web
      development education.
    </p>
    <p>
      <strong>Since 2018,</strong> I’m working with
      <strong>VueJs & NuxtJs</strong> between blows of vacuum cleaner.
    </p>
    <p>
      I feel relieved when things are
      <strong>structured and optimized</strong> in every aspects of my life -
      especially at work - but I swear I am not a robot (at least I pass the
      captcha on websites 🤖!). When I'm not working, I spend my time on video
      games (Metroid Dread 😍) or at the fitness gym (I think my coach
      secretly tries to kill me everyday but still obviously fails 😁).
    </p>
  </v-container>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.about {
  margin: 120px auto;
  z-index: 1000;

  @media only screen and (max-width: 768px) {
    margin: 60px auto;
    padding: 12px 36px !important;
    text-align: justify;
  }
}

h2 {
  margin-bottom: 40px;
}
</style>
