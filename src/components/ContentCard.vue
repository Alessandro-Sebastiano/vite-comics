<template>
    <div class="content-card">
        <div class="content-image">
            <img :src="image" :alt="text">
        </div>
        <span>{{ text }}</span>
    </div>
</template>

<script>

export default {
    name: 'ContentCards',

    props: ['image', 'text'],

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as*;

.content-card {
    width: calc((100% / 6) - 32px);
    margin: 8px 16px;
    min-width: 54px;
    cursor: pointer;


    span {
        display: block;
        height: 50px;
        margin-top: 8px;
        text-transform: uppercase;
        color: $ligth;
        font-weight: 200;
    }
}

.content-image {
    width: 100%;
    max-height: 220px;
    overflow: hidden;

    img {
        width: 100%;
        max-height: 100%;
    }
}
</style>