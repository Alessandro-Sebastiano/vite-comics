<template>
    <div class="footer">
        <div class="component-container">
            <div class="btn">
                <span><a href="#">Sing-up now!</a></span>
            </div>
            <div class="follow">
                <span>Follow us</span>
                <a href="#" v-for="(icon, index) in footerIcons"><img :src="footerIcons[index].imageUrl"
                        :alt="footerIcons[index].alt"></a>
            </div>
        </div>
    </div>
</template>

<script>
export default {

    name: 'FooterComponent',

    data() {

        return {

            footerIcons: [

                {
                    imageUrl: '/images/footer-facebook.png',
                    alt: 'facebook',
                },

                {
                    imageUrl: '/images/footer-twitter.png',
                    alt: 'twitter',
                },

                {
                    imageUrl: '/images/footer-youtube.png',
                    alt: 'youtube',
                },

                {
                    imageUrl: '/images/footer-pinterest.png',
                    alt: 'pinterest',
                },

                {
                    imageUrl: '/images/footer-periscope.png',
                    alt: 'periscope',
                },

            ],

        }

    }

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/_mixins.scss' as *;
@use '../assets/styles/partials/variables' as*;

.footer {
    background-color: $grey;
    padding: 25px 0;
}


.component-container {
    @include general-container;

    display: flex;
    align-items: center;
    justify-content: space-between;
}


.btn {
    border: 2px solid $blue;
    padding: 12px 28px;
    cursor: pointer;
    transition: all 0.6s ease;

    &:hover {
        background-color: $blue;
    }

    a {
        text-decoration: none;
        text-transform: uppercase;
        color: $ligth;
    }
}


.follow {
    display: flex;
    align-items: center;

    span {
        color: $blue;
        font-size: 24px;
        font-weight: 600;
        margin-right: 10px;
        text-transform: uppercase;
    }

    img {
        margin: 0px 8px;
    }
}
</style>