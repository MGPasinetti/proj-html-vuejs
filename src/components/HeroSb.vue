<template>
  <section class="hero-sec">
      <!-- COL-1 -->
      <div>
        <h1>The biggest platform for your growth.</h1>
        <small>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form</small>
        <button>Read More</button>
      </div>

      <!-- COL-2 positioned -->
      <div>
        <img src="../assets/img/27-1.png" alt="hero image">
      </div>
  </section>
</template>

<script>
export default {
    name: 'HeroSb',
}
</script>

<style lang="scss" scoped>
.hero-sec {
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
}
</style>