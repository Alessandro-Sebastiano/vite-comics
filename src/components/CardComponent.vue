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
                    imageUrl: '/images/buy-comics-digital-comics.png',
                    cardText: 'Digital Comics',
                },

                {
                    imageUrl: '/images/buy-comics-merchandise.png',
                    cardText: 'Dc merchandise',
                },

                {
                    imageUrl: '/images/buy-comics-shop-locator.png',
                    cardText: 'Subscription',
                },

                {
                    imageUrl: '/images/buy-comics-subscriptions.png',
                    cardText: 'Comic shop locator',
                },

                {
                    imageUrl: '/images/buy-dc-power-visa.svg',
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
        white-space: nowrap;
    }
}


.card-image {
    max-width: 48px;
    min-width: 28px;

    img {
        width: 100%;
        height: auto;
    }
}
</style>