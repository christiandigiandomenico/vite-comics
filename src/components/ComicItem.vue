<script>
export default {
    name: 'ComicItem',
    props: {
        comicName: String,
        comicImage: String
    },
}
</script>

<template>
    <div class="comic">
        <img :src="comicImage" :alt="comicName">
        <h4>{{ comicName }}</h4>
    </div>
</template>

<style lang="scss">
.comic {
    width: calc(100% / 6);

    img {
        width: 100px;
        height: 100px;
    }

    h4 {
        font-size: 14px;
        font-weight: 400;
    }
}
</style>