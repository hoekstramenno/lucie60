<template>
  <div class="container-masonry">
    <div class="masonry">
      <div class="item">
        <div class="item__content">
          <img src="./assets/jiska.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--medium">
          <img src="./assets/tesse-menno.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--medium">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--large">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--medium">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--large">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--large">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--medium">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--medium">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--large">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--large">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--medium">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--medium">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
      <div class="item">
        <div class="item__content item__content--small">
          <img src="./assets/gerrie-langhaar.png" alt=""/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Gallery'
  }
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css?family=PT+Mono');

  $bg: rgba(255, 92, 4, 0.25);
  $itemBg1: #720026;
  $itemBg2: #CE4257;
  $itemBg3: #FFC093;
  $itemBg4: #FF7F51;
  $counterBg: #222;

  @mixin setColorAndHover($baseColor) {
    color: $baseColor;
    &:hover {
      background: lighten($baseColor, 8%);
    }
  }

  .container-masonry {
    position: relative;
    width: 100%;
    height: 100%;
    background: $bg;
    font-family: "PT Mono", monospace;
    padding: 50px 0;
  }

  .masonry {
    column-count: 1;
    column-gap: 0;
    counter-reset: item-counter;

    @media screen and (min-width: 400px) {
      column-count: 2;
    }

    @media screen and (min-width: 600px) {
      column-count: 3;
    }

    @media screen and (min-width: 800px) {
      column-count: 4;
    }

    @media screen and (min-width: 1100px) {
      column-count: 5;
    }
  }

  .item {
    box-sizing: border-box;
    break-inside: avoid;
    padding: 10px;
    counter-increment: item-counter;

    img {
      width: 100%;
    }

    &__content {
      position: relative;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 220px;
      font-size: 40px;
      color: darken($bg, 5%);
      background: currentColor;
      box-sizing: border-box;
      overflow: hidden;
      @include setColorAndHover($itemBg1);

      &:before {
        position: absolute;
        top: 0;
        left: 0;
        font-size: 13px;
        width: 2em;
        height: 2em;
        line-height: 2em;
        text-align: center;
        font-weight: bold;
        background-color: $counterBg;
        content: counter(item-counter);
      }

      &:after {
        color: darken($bg, 10%);
      }

      &--small {
        @include setColorAndHover($itemBg2);
        height: 100px;
      }

      &--medium {
        @include setColorAndHover($itemBg3);
        height: 175px;
      }

      &--large {
        @include setColorAndHover($itemBg4);
        height: 280px;
      }
    }
  }
</style>
