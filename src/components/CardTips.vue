<template>
    <div class="tips-card">
        <img :src="tipData.srcImg" :alt="tipData.title">
        <div>
            <h4>{{ tipData.title }}</h4>
            <small>{{ tipData.txt }}</small>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CarTips',
    props: {
        tipData: Object,
    },
}
</script>

<style lang="scss" scoped>
.tips-card {
    display: flex;
    gap: 1rem;
    padding: 1.5rem 1rem;
    border: 1px solid lightgrey;
    margin-bottom: 1rem;

    img {
        flex: 0 0 10%;
        height: 3rem;
    }

    &:hover {

    }
}
</style>