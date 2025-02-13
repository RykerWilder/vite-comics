<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppIcons from './components/AppIcons.vue';
import HeroSection from './components/HeroSection.vue';

export default {
  components : {
    AppHeader,
    AppMain,
    HeroSection,
    AppIcons,
    AppFooter
  },

  data() {
    return {
      
    }
  }
}
</script>

<template>

  <AppHeader />
  <HeroSection />
  <AppMain />
  <AppIcons />
  <AppFooter />
  
</template>

<style lang="scss">


</style>
