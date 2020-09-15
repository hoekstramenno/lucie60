<template>
  <div id="app">
    <div class="c-hero">
      <div class="c-hero__content">
        <h1 class="c-hero__headline">Mamma is 60 (bijna 61)</h1>
      </div>
      <div class="c-hero__img-container c-hero--fade-in--img"></div>

    </div>
    <div class="container">
      Gefeliciteerd met je 60 en bijna 61ste verjaardag. Time flies! <br/><br/>
      2020 is niet het jaar waar wij later leuk op terugkijken. Overlijden van oma, Iris en Joey met daarboven een Corona pandemie. We gaan ook met volle overtuiging 2020 afsluiten op 3 oktober en 2021 met 3 maanden verlengen. <br/><br/>
      Na dit hele nare en gekke jaar hebben wij iets bedacht voor jou en pappa. We willen jullie trakteren op een etentje met z'n allen in een leuk restaurant. Altin en Irene zijn er natuurlijk ook bij.   <br/><br/>
      Dit willen wij gaan doen in november 2020. (Duimen dat Corona ons niet tegenhoudt). Pak meteen de agenda en dan gaan we het prikken. <br/>
      <br/>
      Wij houden van jullie!<br/>
      <br/>
      Jiska, Menno<br/>
      Altin, Irene<br/>
      Seppe, Tesse

    </div>
    <restaurants></restaurants>
    <gallery></gallery>
  </div>
</template>

<script>
  import Restaurants from './Restaurants.vue'
  import Gallery from './Gallery.vue'

  export default {
    name      : 'app',
    components: {
      Restaurants,
      Gallery,
    },
  }

</script>

<style lang="scss">
  /*
   * Basic Reset & Styles
   */

  body {
    font-family: 'Source Code Pro', monospace;
    margin: 0;
    padding: 0;
  }

  .container {
    padding: 40px 80px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  p {
    line-height: 1.5em;
  }

  h1+p, p+p {
    margin-top: 10px;
  }


  /*
   * The Good Stuff
   */

  .c-hero {
    height: 100vh;
    overflow: hidden;
    position: relative;
    width: 100%;
  }

  .c-hero__content {
    position: relative;
    top: 50%;
    transform: translateY(-50%);
    max-width: 80%;
    margin-right: auto;
    margin-left: auto;
    z-index: 5;
  }

  .c-hero__headline {
    color: #fff;
    font-size: 6vw;
    font-weight: 200;
    line-height: 1;
    text-align: left;
  }

  .c-hero__img-container {
    background-image: url('assets/hero.png');
    background-size: cover;
    background-position: center center;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  .c-hero--fade-in--img {
    animation-name: heroFadeInImg;
    animation-duration: 5s;
    animation-timing-function: cubic-bezier(0.88, -0.23, 0.29, 1);
    animation-delay: 0s;
    animation-fill-mode: both;
    transform-origin: center;
  }

  @keyframes heroFadeInImg {
    0% {
      opacity: 0;
      transform: scale(1.1);
    }
    100% {
      opacity: 1;
      transform: none;
    }
  }
</style>
