<template>
  <header class="container-sec">
    <!-- LOGO -->
    <div class="logo">
      <img src="../assets/img/logo-2.png" alt="sofbox logo" style="height: 3rem;">
    </div>

    <!-- NAVBAR + SEARCH-i + SHOP-i + BUTTON -->
    <div>
      <NavbarHeader />
      
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

<style>

</style>