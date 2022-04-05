<template>
  <div class="card" :class="{visible: cardData.visible}">
    <div class="card inner">
      <img :src="cardData.srcImg" :alt="cardData.name">
      <span>{{ cardData.name }} - <small>{{ cardData.role }}</small></span>
      <i class="fa-solid fa-quote-right"></i>
      <p>{{ cardData.msg }}</p>
    </div>
    <div class="stack-cards">
      <div></div>
      <div></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardTestimonial',
  props: {
      cardData: Object,
  },
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.card {
  position: relative;
  display: none;

  &.visible {
    display: block;

    .card.inner {
      padding: 2.5rem 2.1rem;
      @include col-layout($direction: column, $align: center);
      background-color: $bkg_color_white;
      position: relative;
      z-index: 2;
      box-shadow: 6px 14px 28px 0px #cfcece;
      border-radius: 3px;
    
      img {
        width: 3rem;
        border-radius: 20rem;
        margin-bottom: 2.5rem;
      }
    
      span {
        margin-bottom: 2rem;
        font-weight: 500;
    
        small {
          font-size: 12px;
        }
      }
    
      i {
        position: absolute;
        top: 4rem;
        font-size: 180px;
        color: rgba(128, 128, 128, .1);
        transform: rotateY(180deg);
      }
    }
    
    .stack-cards {
      position: relative;

      & :first-child {
        position: absolute;
        bottom: -10px;
        left: 10px;
        z-index: 1;
        width: calc(100% - 20px);
        height: 100px;
        background-color: $bkg_color_white;
        box-shadow: 6px 14px 28px 0px #cfcece;
        border-radius: 3px;
      }

      & :last-child {
        position: absolute;
        bottom: -20px;
        left: 20px;
        z-index: 0;
        width: calc(100% - 40px);
        height: 100px;
        background-color: $bkg_color_white;
        box-shadow: 6px 14px 28px 0px #cfcece;
        border-radius: 3px;
      }
    }
  }
}
</style>