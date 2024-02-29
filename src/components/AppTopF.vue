<script>

export default {
    name: 'AppTopF',

    data() {
        return {
            footerLinks: [
              {
                title: "CD COMICS",
                list: [

                  'Character',
                  'Comics',
                  'Movies',
                  'TV',
                  'Games',
                  'Videos',
                  'News'

                ]

              },
              {
                title: "SHOP",
                list: [

                  'Shop DC',
                  'Shop DC Collection',

                ]

              },
              {
                title: "DC",
                list: [

                  'Terms of USe',
                  'Privacy policy (New)',
                  'Ad Choice',
                  'Advertising',
                  'Jobs',
                  'Subscriptions',
                  'CPSC Certificates',
                  'Ratings',
                  'Shop Help',
                  'Contact Us',
                ]

              },

              {
                title: "SITES",
                list: [

                  'DC',
                  'MAD MAgazine',
                  'DC Kids',
                  'DC Universe',
                  'DC Power Visa',
                ]

              },

            ]
        }
    }

}

</script>

<template>
  
  <div id="top-footer">

    <div class="container">

      <div id="link-row">

      <!-- Prima riga di link -->
        <div id="link-row-first" class="links-row">
          <div v-for="linkList in footerLinks.slice(0, 2)" class="links-list">
            <h3>{{ linkList.title }}</h3>
            <ul>
              <li v-for="currentLink in linkList.list">{{ currentLink }}</li>
            </ul>
          </div>
        </div>

        <!-- Seconda riga di link -->
        <div id="link-row-second" class="links-row">
          <div v-for="linkList in footerLinks.slice(2, 4)" class="links-list">
            <h3>{{ linkList.title }}</h3>
            <ul>
              <li v-for="currentLink in linkList.list">{{ currentLink }}</li>
            </ul>
          </div>
        </div>

      </div>

      <!-- Immagine del logo -->
      <div id="img-row">
        <img src="../assets/img/dc-logo-bg.png" alt="DC logo">
      </div>

    </div>
  </div>
  
</template>

<style lang="scss">

@use '../styles/general.scss' as *;

#top-footer {

  width: 100%;

  background-color: $sec_color;
  background-image: url('../assets/img/footer-bg.jpg');
  background-position: cover;
   
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;

      position: relative;

      max-width: 1200px;
      margin: 0 auto;
      padding-bottom: 40px;
      padding-top: 40px;


      #link-row {
        display: flex;
        align-items: flex-start;
        gap: 40px;

        #link-row-first {
          display: flex;
          flex-direction: column;
          gap: 15px;
        }

        #link-row-second {
          display: flex;
          flex-direction: row;
          gap: 40px;
        }

        h3 {
          color: white;
          padding-bottom: 20px;
        }

        li {
          list-style-type: none;
          font-size: 0.7em;
          color: #959595;
          padding-bottom: 8px;
        }
      }

      #img-row {
        position: absolute;
        right: 0px;
        width: 500px;

        img {

          width: 100%;
          
        }

      }
        
    }
}

</style>