<script>

  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import MainLinks from './components/MainLinks.vue';


 export default {
        data() {
            return {

            }
        },

        components: {
          AppHeader,
          AppMain,
          AppFooter,
          MainLinks
        }
    }

</script>

<template>

    
      <AppHeader />
      <AppMain />
      <MainLinks />
      <AppFooter />
    

</template>

<style lang="scss">
  @use "./styles/general.scss" as *;
</style>
