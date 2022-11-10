<template>
    <div class="links-box">
        <div class="component-container">
            <div class="links-columns-box">
                <div class="links-column">
                    <h3>Dc Comics</h3>

                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                    </ul>

                    <h3>Shop</h3>

                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                    </ul>

                </div>

                <div class="links-column">
                    <h3>Dc</h3>

                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                    </ul>

                </div>

                <div class="links-column">
                    <h3>Sites</h3>

                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                    </ul>

                </div>
            </div>
            <div class="background-image">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'LinksComponent',
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/_mixins.scss' as *;
@use '../assets/styles/partials/_variables.scss' as *;

.links-box {
    padding: 54px 0;
    background-image: url('../assets/img/footer-bg.jpg');
    position: relative;
    overflow: hidden
}


.component-container {
    @include general-container;
}

.links-columns-box {
    display: flex;
    align-items: flex-start;
}

.links-column {

    margin-right: 42px;

    h3 {
        color: $ligth;
        margin: 12px 0px;
        text-transform: uppercase;
    }


    ul {
        list-style: none;
    }

    li {
        a {
            text-decoration: none;
            color: $ligth-grey;
            font-weight: 300;
        }
    }



}


.background-image {
    position: absolute;
    top: -56px;
    right: 188px;
}
</style>