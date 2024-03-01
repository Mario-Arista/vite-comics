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
    justify-content: space-between;
    align-items: flex-start; 

    width: calc(100% / 6 - 20px / 6 * 5);
    height: 100%;

    h4 {
        color: white;
        text-transform: uppercase;
        font-size: 0.8em;
        margin-top: 15px;
        margin-bottom: 0px;

        min-height: 1.6em;

    }
    
    img {
        width: 180px;
        height: 180px;
        object-fit: cover;
        object-position: top;
    }

    .price {
        position: absolute;
        right: -5px;
        top: -5px;

        padding: 2px 8px;

        font-size: 0.9em;
        font-weight: bold;

        border-radius: 8px;

        color: white;
        background-color: $primary_color;
    }

    span {

        display: none;
    }


}

@media screen and (max-width: 1200px) {
    .comic {
        width: calc(100% / 4 - 20px / 6 * 5);

        img{
            width: 22vw;
            height: 22vw;
        }
        .price {
            right: -5px;
            top: -5px;
        }
    }
}

@media screen and (max-width: 576px) {
    .comic {
        margin: 0 auto;
        width: 80vw;

        img{
            width: 100%;
            height: 80vw;
        }
    }
}


</style>