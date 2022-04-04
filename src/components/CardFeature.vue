<template>  
    <div>
        <h6>{{ cardData.title }}</h6>
        <img :src="cardData.srcImg" :alt="cardData.title">
    </div>
</template>

<script>
export default {
    name: 'CardFeature',
    props: {
        cardData: Object,
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

</style>