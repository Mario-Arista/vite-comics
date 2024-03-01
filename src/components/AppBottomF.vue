<script>

export default {
    name: 'AppBottomF',

}

</script>

<template>
  
  <div id="bottom-footer">

    <div class="container">

      <button>SIGN-UP NOW!</button>

      <div class="social-isons">
        <span>FOLLOW US</span>
        <img src="/img/footer-facebook.png" alt="Facebook icon">
        <img src="/img/footer-twitter.png" alt="Twitter icon">
        <img src="/img/footer-youtube.png" alt="YouTube icon">
        <img src="/img/footer-pinterest.png" alt="Footer icon">
        <img src="/img/footer-periscope.png" alt="Periscope icon">


      </div>

    </div>

  </div>
  
</template>

<style lang="scss">

@use '../styles/variables.scss' as *;

#bottom-footer {

  width: 100%;

  background-color: #303030;

  padding-top: 25px;
  padding-bottom: 25px;
   
  .container {
    
    justify-content: space-between;

    button {
      background-color: transparent;
      color: white;

      padding: 12px;

      border: $primary_color 1px solid;

      font-size: 1em;
      font-weight: bold;
    }

    .social-isons {
      display: flex;
      justify-content: flex-end;
      align-items: center;
      flex-wrap: wrap;
      gap: 25px;

        span {
          color: $primary_color;
          font-weight: bold;
          font-size: 1.1em;

        }
    }
  }

}
</style>