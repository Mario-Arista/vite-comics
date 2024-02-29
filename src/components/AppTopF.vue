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

      <div v-for="linkList in footerLinks" class="links-list">
          <h3>{{ linkList.title }}</h3>
          <ul>
            <li v-for="currentLink in linkList.list">
              {{ currentLink }}
            </li>
          </ul>
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
   
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;

      max-width: 1200px;


      margin: 0 auto;

      font-size: 1.2em;
      color: white;
        
    }
}

</style>