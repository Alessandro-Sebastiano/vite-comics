<template>
    <div class="card">
        <div class="card-image">
            <img :src="imageUrl" alt="">
        </div>
        <span>{{ cardText }}</span>
    </div>
</template>

<script>



export default {

    name: 'CardComponent',

    data() {
        return {
            imageUrl: './src/assets/img/buy-comics-digital-comics.png',
            cardText: 'DIGITAL COMICS',
        }
    }

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables.scss' as *;

.card {
    display: flex;
    align-items: center;
    margin: 0px 10px;


    span {
        font-weight: 300;
        color: $ligth;
    }
}


.card-image {
    width: 60px;
    margin-right: 8px;

    img {
        width: 100%;
        height: auto;
    }
}
</style>