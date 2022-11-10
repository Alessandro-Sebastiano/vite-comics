<template>
    <div class="cards-box">
        <div class="component-container">
            <CardComponent />
        </div>
    </div>
</template>

<script>

import CardComponent from './CardComponent.vue';

export default {

    name: 'CardBox',

    components: {
        CardComponent,
    }

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/_mixins.scss' as *;
@use '../assets/styles/partials/variables' as*;


.cards-box {
    background-color: $blue;
    padding: 34px 0;
}

.component-container {
    @include general-container;

    display: flex;
    align-items: center;
    justify-content: space-around;
}
</style>