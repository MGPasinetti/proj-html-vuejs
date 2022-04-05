<template>
  <section class="features-sec">
      <img src="../assets/img/14.png" alt="">
      <div class="container-sec">
          <div class="header-group">
              <div>
                    <h2>Popular features that your business needs</h2>
                    <small>Faff about only a quid blower I don't want no agro bleeding chimney <br> pot burke tosser cras nice one boot fanny.!</small>
              </div>
              <button>Explore More Feature</button>
          </div>
          <div class="grid-cards">
              <CardFeature v-for="card in arrFeatCards" :key="card.title" :card-data="card"/>
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
    },
    data() {
        return {
            arrFeatCards: [
                {
                    title: 'Customized Invoices',
                    srcImg: require('../assets/img/feat-1.png')
                },
                {
                    title: 'Stock Management',
                    srcImg: require('../assets/img/feat-2.png')
                },
                {
                    title: 'Receivable & Payables',
                    srcImg: require('../assets/img/feat-3.png')
                },
                {
                    title: 'Manage Buying',
                    srcImg: require('../assets/img/feat-4.png')
                },
                {
                    title: 'Powerful & Secure',
                    srcImg: require('../assets/img/feat-5.png')
                },
                {
                    title: 'Fastest Return Filing',
                    srcImg: require('../assets/img/feat-3.png')
                },
                {
                    title: 'Monthly Detailed',
                    srcImg: require('../assets/img/feat-6.png')
                },
                {
                    title: 'Product Management',
                    srcImg: require('../assets/img/feat-7.png')
                },
            ],
        };
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.features-sec {
    position: relative;
    
    img {
        height: calc(392px + 8rem);
        position: absolute;
        left: -250px;
        top: -8rem;
        z-index: -1;
    }

    .container-sec {
    background-color: transparent;

        .header-group {
            @include flex-layout;
            margin-bottom: 3rem;

            div {
                flex: 0 0 70%;
            }

            button {
                margin: 2rem;
            }
        }

        .grid-cards {
            @include flex-layout;
            gap: 1.5rem;

            & > * {
                width: calc((100% - 4.5rem) / 4);
            }
        }
    }
}
</style>