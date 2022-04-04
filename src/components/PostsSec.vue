<template>
  <section>
      <div class="container-sec">
            <h1>Latest Posts</h1>
            <small>If you are planning on developing a product landing.</small>
            <div class="posts-grid">
                <CardPost v-for="post in arrPosts" :key="post.srcImg" :card-data="post"/>
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
                    name: 'Julia Aann',
                    role: 'COO Sofbox',
                    msg: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.' 
                },
                {
                    srcImg: require('../assets/img/18.jpg'),
                    name: 'Mac Znder',
                    role: 'Manager Sofbox',
                    msg: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.' 
                },
                {
                    srcImg: require('../assets/img/17.jpg'),
                    name: 'Max Fletcher',
                    role: 'IT-Manager Sofbox',
                    msg: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.' 
                },
            ],
        };
    }
}
</script>

<style lang="scss" scoped>

</style>