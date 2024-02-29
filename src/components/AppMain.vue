<script>

export default {
    name: 'AppMain',

}

</script>

<template>
  
    <main>

        <div class="container">Content goes here!</div>

    </main>

  
</template>

<style lang="scss">

@use '../styles/general.scss' as *;

main {

    width: 100%;

    background-color: $sec_color;
   
    .container {
        max-width: 1200px;

        margin: 0 auto;

        padding-top: 50px;
        padding-bottom: 50px;

        font-size: 1.2em;
        color: white;
        
    }
}

</style>