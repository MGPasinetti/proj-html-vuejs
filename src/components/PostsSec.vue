<template>
  <section class="post-sec">
      <div class="container-sec jumbotron">
            <div class="header-sec">
                <h2>Latest Posts</h2>
                <small>If you are planning on developing a product landing.</small>
            </div>
            <div class="posts-grid">
                <CardPost class="card-post" v-for="post in arrPosts" :key="post.srcImg" :post-data="post"/>
            </div>
      </div>
  </section>
</template>

<script>
import CardPost from './CardPost.vue';

export default {
    name: 'PostsSec',
    components: {
       CardPost, 
    },
    data() {
        return {
            arrPosts: [
                {
                    srcImg: require('../assets/img/19.jpg'),
                    date: 'November 28, 2019',
                    title: 'Life Lack Meaning',
                    text: 'It is a long established fact that a reader will be distracted by the readable.' 
                },
                {
                    srcImg: require('../assets/img/18.jpg'),
                    date: 'November 29, 2019',
                    title: 'Life Lack Meaning',
                    text: 'It is a long established fact that a reader will be distracted by the readable.' 
                },
                {
                    srcImg: require('../assets/img/17.jpg'),
                    date: 'November 30, 2019',
                    title: 'Life Lack Meaning',
                    text: 'It is a long established fact that a reader will be distracted by the readable.' 
                },
            ],
        };
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.container-sec {
    margin-top: -8rem;
    @include col-layout($direction: column, $align: center);

    .posts-grid {
        display: flex;
        flex-wrap: wrap;
        gap: 1.5rem;

        .card-post {
            width: calc((100% - 3rem) / 3);
        }
    }
}
</style>