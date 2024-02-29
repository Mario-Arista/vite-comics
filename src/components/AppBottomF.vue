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
        <img src="../assets/img/footer-facebook.png" alt="Facebook icon">
        <img src="../assets/img/footer-twitter.png" alt="Twitter icon">
        <img src="../assets/img/footer-youtube.png" alt="YouTube icon">
        <img src="../assets/img/footer-pinterest.png" alt="Footer icon">
        <img src="../assets/img/footer-periscope.png" alt="Periscope icon">


      </div>

    </div>

  </div>
  
</template>

<style lang="scss">

@use '../styles/general.scss' as *;

#bottom-footer {

  width: 100%;
  z-index: 3;

  background-color: #303030;

  padding-top: 25px;
  padding-bottom: 25px;
   
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;

    margin: 0 auto;

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