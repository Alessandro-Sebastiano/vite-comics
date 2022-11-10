<template>
    <div class="header">
        <div class="component-container">
            <div class="header-logo">
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
            </div>

            <div class="menu-list">
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
                </ul>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'HeaderComponent',
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/_mixins.scss' as *;
@use '../assets/styles/partials/variables' as*;


.component-container {
    @include general-container;

    display: flex;
    align-items: center;
    justify-content: space-between;
}


.menu-list {

    height: auto;

    ul {
        list-style: none;
        display: flex;
        align-items: center;


        li {
            padding: 4px 16px;

            a {
                text-decoration: none;
                color: $dark;

                &:hover {
                    color: $blue;
                }
            }
        }

    }
}
</style>