<template>
    <div class="content">
        <div class="component-container">
            <ContentCard v-for="(item, index) in cards" :image="item.thumb" :text="item.series" />
        </div>
    </div>
</template>

<script>
import ContentCard from './ContentCard.vue';
import json from '../data/dc-comics.json';

export default {
    name: 'ContentComponent',
    components: {
        ContentCard,
    },

    data() {
        return {
            cards: json,
        }
    },

    mounted() {
        console.log(this.cards);
    }

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/_mixins.scss' as *;
@use '../assets/styles/partials/variables' as*;


.content {
    background-color: $dark;
    padding: 42px 0px;
}

.component-container {
    @include general-container;

    display: flex;
    flex-wrap: wrap;
    align-items: center;

    h2 {
        color: $ligth;
    }
}
</style>