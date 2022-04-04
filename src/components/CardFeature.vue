<template>  
    <div>
        <h1>{{ title }}</h1>
        <img :src="{img}" :alt="title">
    </div>
</template>

<script>
export default {
    name: 'CardFeature',
    props: {
        title: String,
        img: String,
    }
}
</script>

<style lang="scss" scoped>

</style>