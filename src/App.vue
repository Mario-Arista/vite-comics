<script>
import AppNav from './components/AppNav.vue';
import AppMain from './components/AppMain.vue';
import AppFeatures from './components/AppFeatures.vue';
import AppFooter from './components/AppFooter.vue';

export default {

  components: {
    AppNav,
    AppMain,
    AppFeatures,
    AppFooter,
  }

}
</script>

<template>
    <AppNav></AppNav>

    <AppMain></AppMain>

    <AppFeatures></AppFeatures>

    <AppFooter></AppFooter>

</template>

<style lang="scss">

@use './styles/general.scss' as *;

</style>