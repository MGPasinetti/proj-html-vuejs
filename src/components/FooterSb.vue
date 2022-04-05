<template>
  <footer>
      <div class="container-sec">
        <div class="col">
            <img class="logo" src="../assets/img/35.png" alt="SofBox logo">
            <small>It is a long established fact that a reader will be distracted by the readable content.</small>
            <small>Copyright @ <a href="#">Sofbox</a></small>
        </div>
        <div class="col" v-for="(list, index) in arrLists" :key="index">
            <ListFooter :list-data="list"/>
        </div>
      </div>
  </footer>
</template>

<script>
import ListFooter from './ListFooter.vue';

export default {
    name: 'FooterSb',
    components: {
       ListFooter, 
    },
    data() {
        return {
            arrLists: [
                {
                    title: 'Menu',
                    arrLinks: [
                        'About Us',
                        'Theme',
                        'Features',
                        'Pricing',
                        'Blog',
                    ],
                },
                {
                    title: 'About Us',
                    arrLinks: [
                        'About Sofbox',
                        'Roadmap',
                        'How it Work',
                        'Team',
                        'News',
                    ],
                },
                {
                    title: 'Quick Links',
                    arrLinks: [
                        'About Us',
                        'Theme',
                        'Features',
                        'Pricing',
                        'Blog',
                    ],
                },
            ],
        };
    },
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

footer {
    border-top: 1px solid $border_color_lightgrey;
    padding: 3rem 0 5rem 0;

    .container-sec {
        @include flex-layout($justify: space-between, $align: flex-start, $wrap: nowrap);
        gap: 4rem;
    
        .col {
            @include col-layout($direction: column, $align: flex-start);
            width: calc(100% / 4);
    
            .logo {
                width: 8rem;
                margin-bottom: .5rem;
            }

            small {
                font-size: 12px;
            }

            a {
                color: $txt_color_blue;
            }
        }
    }
}
</style>