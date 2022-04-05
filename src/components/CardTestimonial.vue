<template>
  <div class="card">
    <img :src="cardData.srcImg" :alt="cardData.name">
    <span><strong>{{ cardData.name }}</strong> - <small>{{ cardData.role }}</small></span>
    <i class="fa-solid fa-quote-right"></i>
    <p>{{ cardData.msg }}</p>
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
  padding: 2.1rem;
  @include col-layout($direction: column, $align: center);
  background-color: $bkg_color_white;
  position: relative;
  box-shadow: 6px 14px 28px 0px #cfcece;

  img {
    width: 3rem;
    border-radius: 20rem;
    margin-bottom: 2.5rem;
  }

  span {
    margin-bottom: 2rem;

    small {
      font-size: 12px;
    }
  }

  i {
    position: absolute;
    top: 4rem;
    font-size: 180px;
    color: rgba(128, 128, 128, .2);
    transform: rotateY(180deg);
  }

  p {
    font-size: 14px;
    font-weight: 400;
    color: $txt_color_grey;
    line-height: 1.5;
  }
}
</style>