<script>
import digitalComicsImage from "../assets/img/buy-comics-digital-comics.png";
import merchImage from "../assets/img/buy-comics-merchandise.png";
import subscriptionImage from "../assets/img/buy-comics-subscriptions.png";
import shopLocatorImage from "../assets/img/buy-comics-shop-locator.png";
import powerVisaImage from "../assets/img/buy-dc-power-visa.svg";

export default {

  name: 'AppFeatures',

  data() {
    return {
      features: [
        {
          image: digitalComicsImage,
          text: "DIGITAL COMICS",
        },
        {
          image: merchImage,
          text: "DC MERCHANDISING",
        },
        {
          image: subscriptionImage,
          text: "SUBSCRIPTION",
        },
        {
          image: shopLocatorImage,
          text: "COMIC SHOP LOCATOR",
        },
        {
          image: powerVisaImage,
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
        <img :src="currenFeature.image" :alt="currenFeature.text">
        <span>{{ currenFeature.text }}</span>
      </div>
    </div>
    
  </div>

  
</template>

<style lang="scss">

@use '../styles/general.scss' as *;

#AppFeatures {
    background-color: $primary_color;
    color: white;
    width: 100%;

    .container {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 65px;

      max-width: 1200px;

      margin: 0 auto;

      padding-top: 45px;
      padding-bottom: 45px;

      color: white;
      
        .single-feature {
          display: flex;
          align-items: center;
          gap: 10px;

            img {
              width: 45px;
              height: auto;
            }

            span {
              font-size: 0.8em;
            }

        }
    }
}


</style>