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
@import "../assets/styles/style.scss";

.tips-card {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 1.5rem 1rem;
    border: 1px solid transparent;

    img {
        flex: 0 0 10%;
        height: 3rem;
    }

    &:hover {
        border: 1px solid $border_color_whitesmoke2; 
        box-shadow: 10px 14px 28px 0px #cfcece;
        
        h4 {
            color: $txt_color_blue;
        }
    }
}
</style>