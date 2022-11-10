<template>
    <div class="content">
        <div class="component-container">
            <h2>{{ contenTitle }}</h2>
        </div>
    </div>
</template>

<script>



export default {

    name: 'ContentComponent',

    data() {
        return {
            contenTitle: '--> Content goes here <--'
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/_mixins.scss' as *;
@use '../assets/styles/partials/variables' as*;


.content {
    background-color: $dark;
    padding: 26px 0px;
}

.component-container {
    @include general-container;

    h2 {
        color: $ligth;
    }
}
</style>