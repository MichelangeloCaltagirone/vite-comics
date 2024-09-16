<script>

  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';

 export default {
        data() {
            return {

            }
        },

        components: {
          AppHeader,
          AppMain,
          AppFooter
        }
    }

</script>

<template>

    <div class="container">
      <AppHeader />
      <AppMain />
      <AppFooter />
    </div>

</template>

<style lang="scss" scoped>
  @use "./styles/general.scss";

  .container {
    max-width: 1000px;
    margin: 0 auto;
  }

</style>
