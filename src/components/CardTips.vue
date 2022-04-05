<template>
    <div class="tips-card" @click="setActiveTip" :class="{active: activeTip}">
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
    data() {
        return {
            activeTip: false,
        };
    },
    methods: {
        setActiveTip() {
            return this.activeTip = !this.activeTip;
        },
    }
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
    cursor: pointer;

    img {
        flex: 0 0 10%;
        height: 3rem;
    }

    &:hover {
        border: 1px solid $border_color_whitesmoke2; 
        box-shadow: 6px 14px 28px 0px #cfcece;
        
        h4 {
            color: $txt_color_blue;
        }
    }

    &.active {
        border: 1px solid $border_color_whitesmoke2; 
        box-shadow: 6px 14px 28px 0px #cfcece;
        
        h4 {
            color: $txt_color_blue;
        }
    }
}
</style>