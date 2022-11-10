<template>
    <HeaderComponent />
    <ContentComponent />
    <CardsBox />
    <LinksComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import ContentComponent from './components/ContentComponent.vue';
import CardsBox from './components/CardsBox.vue';
import LinksComponent from './components/LinksComponent.vue';

export default {
    components: {
        HeaderComponent,
        ContentComponent,
        CardsBox,
        LinksComponent,
    }
}
</script>

<style lang="scss" scoped>

</style>