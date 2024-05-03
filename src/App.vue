<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppIcons from './components/AppIcons.vue';

export default {
  components : {
    AppIcons,
    AppHeader,
    AppMain,
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
  <AppMain />
  <AppIcons />
  <AppFooter />
  
</template>

<style lang="scss">


</style>
