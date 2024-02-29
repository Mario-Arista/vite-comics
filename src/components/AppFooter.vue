<script>
import AppTopF from './AppTopF.vue';
import AppBottomF from './AppTopF.vue'

export default {
    name: 'AppFooter',

    components: {
        AppTopF,
        AppBottomF,
    },

}

</script>

<template>
  
    <footer>
        <AppTopF></AppTopF>

        <AppBottomF></AppBottomF>
    </footer>
  
</template>

<style lang="scss">

</style>