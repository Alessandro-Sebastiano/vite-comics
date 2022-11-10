<template>
    <HeaderComponent />
    <ContentComponent />
    <CardsBox />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import ContentComponent from './components/ContentComponent.vue';
import CardsBox from './components/CardsBox.vue';

export default {
    components: {
        HeaderComponent,
        ContentComponent,
        CardsBox,
    }
}
</script>

<style lang="scss" scoped>

</style>