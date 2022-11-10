<template>
    <div class="card" v-for="(el, index) in cards">
        <div class="card-image">
            <img :src="cards[index].imageUrl" :alt="cards[index].cardText">
        </div>
        <span>{{ cards[index].cardText }}</span>
    </div>
</template>

<script>



export default {

    name: 'CardComponent',

    data() {
        return {
            cards: [

                {
                    imageUrl: './src/assets/img/buy-comics-digital-comics.png',
                    cardText: 'Digital Comics',
                },

                {
                    imageUrl: './src/assets/img/buy-comics-merchandise.png',
                    cardText: 'Dc merchandise',
                },

                {
                    imageUrl: './src/assets/img/buy-comics-shop-locator.png',
                    cardText: 'Subscription',
                },

                {
                    imageUrl: './src/assets/img/buy-comics-subscriptions.png',
                    cardText: 'Comic shop locator',
                },

                {
                    imageUrl: './src/assets/img/buy-dc-power-visa.svg',
                    cardText: 'Dc power visa',
                },

            ],
        }
    },

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables.scss' as *;

.card {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    margin: 0px 10px;
    cursor: pointer;
    max-height: 65px;


    span {
        font-weight: 300;
        color: $ligth;
        margin-left: 10px;
        text-transform: uppercase;
    }
}


.card-image {
    width: 55px;

    img {
        width: 100%;
        height: auto;
    }
}
</style>