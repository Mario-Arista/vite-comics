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

@use '../styles/variables.scss' as *;

main {

    width: 100%;

    background-color: $sec_color;
   
    .container {

        padding-top: 50px;
        padding-bottom: 50px;

        font-size: 1.2em;
        color: white;
        
    }
}

</style>