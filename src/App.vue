<template>
    <HeaderComponent />
    <JumbotronComponent />
    <ContentComponent />
    <CardsBox />
    <LinksComponent />
    <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import ContentComponent from './components/ContentComponent.vue';
import CardsBox from './components/CardsBox.vue';
import LinksComponent from './components/LinksComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
import JumbotronComponent from './components/JumbotronComponent.vue';

export default {
    components: {
        HeaderComponent,
        ContentComponent,
        CardsBox,
        LinksComponent,
        FooterComponent,
        JumbotronComponent,
    }
}
</script>

<style lang="scss" scoped>

</style>