<template>
    <section class="container-sec tips-tricks-sec">
      <!-- COL-1 -->
      <div class="col">
            <h2>Get tips tricks on how to skyrocket your sales.</h2>
            <small>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</small>
            <CardTips v-for="tip in arrTips" :key="tip.title" :tip-data="tip"/>
      </div>

      <!-- COL-2 -->
      <img src="../assets/img/509.jpeg" alt="">
  </section>
</template>

<script>
import CardTips from './CardTips.vue';

export default {
    name: 'TipsTricksSec',
    components: {
        CardTips,
    },
    data() {
        return {
            arrTips: [
                {
                    srcImg: require('../assets/img/510.png'),
                    title: 'Reporting Analysis',
                    txt: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout',
                },
                {
                    srcImg: require('../assets/img/511.png'),
                    title: 'Technical SEO Audit',
                    txt: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout',
                },
            ],
        };
    },
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.tips-tricks-sec {
    @include flex-layout($justify: space-between, $align: none, $wrap: nowrap);
    gap: 2rem;

    & > * {
        flex: 0 0 40%
    }

   .col {
       @include col-layout;
   }

   img {
       max-width: 500px;
   }
}
</style>