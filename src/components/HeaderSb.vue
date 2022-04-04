<template>
  <header class="container-sec">
    <!-- LOGO -->
    <div class="logo">
      <img src="../assets/img/logo-2.png" alt="sofbox logo" style="height: 3rem;">
    </div>

    <!-- NAVBAR + SEARCH-i + SHOP-i + BUTTON -->
    <div>
      <NavbarHeader />
      <div class="icons">
        <a href="#"><i class="fa-solid fa-magnifying-glass"></i></a>
        <a href="#"><i class="fa-solid fa-cart-shopping"></i><span>0</span></a> <!-- + number items rounded -->
      </div>
      <button>Get Started</button>
    </div>
  </header>
</template>

<script>
import NavbarHeader from './NavbarHeader.vue';

export default {
  name: 'HeaderSb',
  components: {
    NavbarHeader,
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

header {
  @include flex-layout;

  div:last-child {
    flex: 0 0 65%;
    @include flex-layout;

    .icons {
      & .fa-magnifying-glass{
        margin-right: 1.5rem;
      }

      a:last-child span {
        padding: .2rem .4rem;
        line-height: 1;
        background-color: rgba($bkg_color_blue, .8);
        color: $txt_color_white;
        font-size: 9px;
        border-radius: 20rem;
        position: relative;
        top: -10px;
        left: -6px;
      }
    }
  }
}
</style>