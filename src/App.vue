<template>
    <HeaderComponent />
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


export default {
    components: {
        HeaderComponent,
        ContentComponent,
        CardsBox,
        LinksComponent,
        FooterComponent,
    }
}
</script>

<style lang="scss" scoped>

</style>