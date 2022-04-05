<template>
    <section class="container-sec tips-tricks-sec">
      <!-- COL-1 -->
      <div class="col">
            <h2>Get tips tricks on how to skyrocket your sales.</h2>
            <small>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</small>
            <CardTips class="tips-card" v-for="(tip, index) in arrTips" :key="index" :tip-data="(tip)" @click="setActiveTip(index)" :class="{active: index == activeTip}" />
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
            activeTip: 0,
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
    methods: {
        setActiveTip (index) {
            this.activeTip = index;
        },
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.tips-tricks-sec {
    @include flex-layout($justify: space-between, $align: center, $wrap: nowrap);

   .col {
       @include col-layout;
        flex: 0 0 51%;
   }

   img {
       max-height: 350px;
   }

}
.tips-card.active {
    border: 1px solid $border_color_whitesmoke2; 
    box-shadow: 6px 14px 28px 0px #cfcece;
    
    h4 {
        color: $txt_color_blue;
    }
}
</style>