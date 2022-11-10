<template>
    <div class="footer">
        <div class="component-container">
            <div class="btn">
                <span><a href="#">Sing-up now!</a></span>
            </div>
            <div class="follow">
                <span>Follow us</span>
                <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
                <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
                <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
                <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
            </div>
        </div>
    </div>
</template>

<script>
export default {

    name: 'FooterComponent',

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