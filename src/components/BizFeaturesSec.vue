<template>
  <section class="features-sec">
      <img src="../assets/img/14.png" alt="">
      <div class="container-sec">
          <div class="header-group">
              <div>
                    <h1>Popular features that your business needs</h1>
                    <small>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</small>
              </div>
              <button>Explore More Feature</button>
          </div>
          <div class="grid-cards">
              <CardFeature title="Customized Invoices" img="../assets/img/feat-1.png"/>
          </div>
      </div>
  </section>
</template>

<script>
import CardFeature from './CardFeature.vue';

export default {
    name: 'BizFeaturesSec',
    components: {
        CardFeature,
    }
}
</script>

<style lang="scss" scoped>
.features-sec {
    position: relative;
    min-height: 653px;
    img {
        position: absolute;
        left: -325px;
    }

    .header-group {
        display: flex;
        align-items: center;
    }
}
</style>