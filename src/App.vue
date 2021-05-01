<template>
  <div class="outer-wrapper">
      <div class="container">
        <Navbar></Navbar>
        <HeroSection></HeroSection>
      </div>
      <IntroSection></IntroSection>
      <div class="container">
        <SkillsSection></SkillsSection>
      </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
import IntroSection from './components/IntroSection.vue'
import SkillsSection from './components/SkillsSection.vue'


export default {
  name: 'App',
  components: {
    Navbar,
    HeroSection,
    IntroSection,
    SkillsSection
  }
}
</script>

<style lang="scss">

</style>
