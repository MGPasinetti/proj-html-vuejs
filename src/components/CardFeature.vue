<template>  
    <div>
        <h1>{{ cardData.title }}</h1>
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

</style>