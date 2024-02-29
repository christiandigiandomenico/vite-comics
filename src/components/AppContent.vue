<script>
import AppMerchandise from './AppMerchandise.vue';

export default {
    name: "AppContent",
    components: {
        AppMerchandise,
    }
}
</script>

<template>
    <div class="main-content">

        <div class="text-content">
            Content goes here
        </div>

    </div>
    <AppMerchandise></AppMerchandise>
</template>

<style lang="scss">
.main-content {
    background-color: #1c1c1c;

    .text-content {
        font-size: 42px;
        padding: 24px;
        max-width: 1270px;
        margin: auto;
    }
}
</style>