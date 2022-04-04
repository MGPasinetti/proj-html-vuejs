<template>
  <section class="hero-sec">
      <!-- COL-1 -->
      <div>
        <h1>The biggest platform for your growth.</h1>
        <small>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form</small>
        <button>Read More</button>
      </div>

      <!-- COL-2 positioned -->
      <img src="../assets/img/27-1.png" alt="hero image">
  </section>
</template>

<script>
export default {
    name: 'HeroSb',
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.hero-sec {
  max-width: 1100px;
  height: 400px;
  margin: 0 auto;
  display: flex;
  background-color: $bkg_color_lilla;
  padding: 3rem;
  border-radius: 5px;
  margin-bottom: 7rem;

  & :first-child {
    @include col-layout;
    margin-bottom: 1rem;
    flex: 0 0 40%;
    min-width: 430px;

    & button {
      height: fit-content;
    }
  }

  & :last-child {
    flex-shrink: 1;
    height: 390px;
  }  
}
</style>