<script>
import AppNav from './components/AppNav.vue';
import AppMain from './components/AppMain.vue';
import AppFeatures from './components/AppFeatures.vue';
import AppTopF from './components/AppTopF.vue';
import AppBottomF from './components/AppBottomF.vue';


export default {

  components: {
    AppNav,
    AppMain,
    AppFeatures,
    AppTopF,
    AppBottomF,
  }

}
</script>

<template>
    <AppNav></AppNav>

    <AppMain></AppMain>

    <AppFeatures></AppFeatures>

    <footer>
      <AppTopF></AppTopF>
      <AppBottomF></AppBottomF>
    </footer>

</template>

<style lang="scss">

@use './styles/general.scss' as *;

</style>