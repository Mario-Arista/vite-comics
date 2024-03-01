<script>

export default {

  name: 'AppFeatures',

  data() {
    return {
      features: [
        {
          image: "/img/buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          image: "/img/buy-comics-merchandise.png",
          text: "DC MERCHANDISING",
        },
        {
          image: "/img/buy-comics-subscriptions.png",
          text: "SUBSCRIPTION",
        },
        {
          image: "/img/buy-comics-shop-locator.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          image: "/img/buy-dc-power-visa.svg",
          text: "DC POWER VISA",
        },
      ]

    }
  }

}

</script>

<template>
  
  <div id="AppFeatures">

    <div class="container">
      <div 
        class="single-feature"
        v-for="currenFeature in features"
      >
        <div class="img-container">
          <img :src="currenFeature.image" :alt="currenFeature.text">
        </div>
        
        <h3>{{ currenFeature.text }}</h3>
      </div>
    </div>
    
  </div>

  
</template>

<style lang="scss">

@use '../styles/variables.scss' as *;

#AppFeatures {
    background-color: $primary_color;
    color: white;
    width: 100%;

    .container {
      
      justify-content: center;
      flex-wrap: wrap;
      gap: 65px;
      padding-top: 45px;
      padding-bottom: 45px;

      
        .single-feature {
          display: flex;
          align-items: center;
          gap: 10px;

          .img-container {
            display: flex;
            align-items: center;
            justify-content: center;

            height: 50px;

            img {
              height: 100%;
              max-width: 50px;
              
            }

          }

          h3 {
            font-size: 0.8em;
          }

        }
    }
}


</style>