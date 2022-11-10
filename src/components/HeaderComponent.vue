<template>
    <div class="header">
        <div class="component-container">
            <div class="header-logo">
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
            </div>

            <div class="menu-list">
                <ul>
                    <li v-for="(item, index) in menuItems" :key="index" @click="activeLink(index)"><a
                            :class="{ active: menuItems[index].itemActive }" href="#">{{ menuItems[index].itemText
                            }}</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'HeaderComponent',

    data() {

        return {

            menuItems: [

                {
                    itemText: 'Characters',
                    itemActive: true,
                },

                {
                    itemText: 'Comics',
                    itemActive: false,
                },

                {
                    itemText: 'Movies',
                    itemActive: false,
                },

                {
                    itemText: 'Tv',
                    itemActive: false,
                },

                {
                    itemText: 'Games',
                    itemActive: false,
                },

                {
                    itemText: 'Collectibles',
                    itemActive: false,
                },

                {
                    itemText: 'Videos',
                    itemActive: false,
                },

                {
                    itemText: 'Fans',
                    itemActive: false,
                },

                {
                    itemText: 'News',
                    itemActive: false,
                },

                {
                    itemText: 'Shop',
                    itemActive: false,
                },

            ],

        }

    },

    methods: {

        activeLink(index) {
            this.menuItems.forEach((element) => {
                element.itemActive = false;
            })
            this.menuItems[index].itemActive = true;
        }

    },

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

    ul {
        list-style: none;
        display: flex;
        align-items: center;


        li {
            padding: 4px 16px;

            a {
                text-decoration: none;
                text-transform: uppercase;
                color: $dark;
                border-bottom: 3px solid $blue;
                padding: 10px 0;


                &:hover {
                    color: $blue;
                }


                &::after {
                    content: '';
                    display: block;
                    width: 100%;
                    height: 3px;
                    background-color: $ligth;
                    position: relative;
                    bottom: -10px;
                    float: right;
                }
            }

        }


        .active {
            color: $blue;

            &::after {
                width: 1%;
                transition: all 0.4s ease;
            }
        }

    }
}
</style>