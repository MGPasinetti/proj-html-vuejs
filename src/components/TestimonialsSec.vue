<template>
  <section>
    <div class="big-sec">
      <img src="../assets/img/15.png" alt="">
      <div class="container-sec">
          <h1>Our Testimonials</h1>
          <small>If you are planning on developing a product landing app or website, take a look at this beautiful-cafted</small>
      </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'TestimonialsSec',
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.big-sec {
    background: linear-gradient(#F0F7FF, $bkg_color_white);
    // background: linear-gradient(0deg, blue, green 40%, red);

    .container-sec {
        position: relative;
        top: -70px;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: transparent;
    }
}
</style>