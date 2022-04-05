<template>
  <section class="testimonial-sec">
    <div class="big-sec">
      <img src="../assets/img/15.png" alt="">
      <div class="container-sec">
            <div class="header-sec">
                <h2>Our Testimonials</h2>
                <small>If you are planning on developing a product landing app or website, take a look at this beautiful-cafted</small>
            </div>
            <div class="testimonials-grid">
                <CardTestimonial v-for="card in arrTestimonials" :key="card.name" :card-data="card"/>
            </div>
            <div class="square-group" style="display: flex; gap: .3rem;">
                <div class="first-square" style="width: .5rem; height: .5rem; background-color: #377DFF; border-radius: 2px;"></div>
                <div class="second-square" style="width: .5rem; height: .5rem; background-color: black; border-radius: 2px;"></div>
            </div>
      </div>
    </div>
  </section>
</template>

<script>
import CardTestimonial from './CardTestimonial.vue';

export default {
    name: 'TestimonialsSec',
    components: {
        CardTestimonial,
    },
    data() {
        return {
            arrTestimonials: [
                {
                    srcImg: require('../assets/img/26.jpeg'),
                    name: 'Julia Aann',
                    role: 'COO Sofbox',
                    msg: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.' 
                },
                {
                    srcImg: require('../assets/img/27.jpeg'),
                    name: 'Mac Znder',
                    role: 'Manager Sofbox',
                    msg: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.' 
                },
                // {
                //     srcImg: require('../assets/img/25.jpeg'),
                //     name: 'Max Fletcher',
                //     role: 'IT-Manager Sofbox',
                //     msg: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.' 
                // },
            ],
        };
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.big-sec {
    background: linear-gradient(.50turn, $bkg_color_lilla, 100px, $bkg_color_white);

    .container-sec {
        position: relative;
        top: -100px;
        @include col-layout($direction: column, $align: center);
        background-color: transparent;

        .testimonials-grid {
            display: flex;
            gap: 3rem;
            margin-bottom: 3rem;
        }
    }
}
</style>