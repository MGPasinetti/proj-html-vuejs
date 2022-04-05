<template>  
    <div>
        <h4>{{ cardData.title }}</h4>
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

div {
    padding: 1rem; 
    border: 1px solid $border_color_whitesmoke2;
    box-shadow: 6px 14px 28px 0px #cfcece;
    border-radius: 3px;

    img {
        width: 3rem;
        height: 3rem;
        margin-bottom: 1rem;
        border-radius: 5rem;
    }

    &:hover {
        background-color: $bkg_color_lightgreen;
        border: 1px solid $bkg_color_lightgreen;
        box-shadow: 6px 14px 28px 0px $bkg_color_lightgreen;
        color: white;
    }
}

</style>