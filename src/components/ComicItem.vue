<script>

export default {
    name: 'ComicItem',

    props: {

        ComicImage: String,
        ComicPrice: String,
        ComicType: String,
        ComicSeries: String,

    },


}

</script>

<template>
  
    <div class="comic">

        <img :src="ComicImage" :alt="ComicSeries">

        <h4>{{ ComicSeries }}</h4>

        <span>{{ ComicType }}</span>

        <div class="price">{{ ComicPrice }}</div>
    </div>

  
</template>

<style lang="scss">

@use '../styles/variables.scss' as *;

.comic {
    position: relative;

    display: flex;
    flex-direction: column;
    align-items: center;

    width: calc(100% / 6 - 20px / 6 * 5);

    h4 {
        color: white;
        text-transform: uppercase;
        font-size: 0.9em;

        padding-top: 10px;
    }
    
    img {
        display: block;
        width: 180px;
        height: 180px;
        object-fit: cover;
        object-position: top;
    }

    .price {
        position: absolute;
        left: -5px;
        top: -5px;

        padding: 2px 4px;

        font-size: 0.8em;
        font-weight: bold;

        color: white;
        background-color: $primary_color;
    }

    span {

        display: none;
    }


}

</style>