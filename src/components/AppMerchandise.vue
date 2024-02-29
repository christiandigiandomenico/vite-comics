<script>
export default {
    name: "AppMerchandise",

    data() {
        return {
            merchandise: [
                {
                    name: "DITIGAL COMICS",
                    url: '/img/buy-comics-digital-comics.png'
                },
                {
                    name: "DC MERCHANDISE",
                    url: '/img/buy-comics-merchandise.png'
                },
                {
                    name: "SUBSCRIPTION",
                    url: '/img/buy-comics-subscriptions.png'
                },
                {
                    name: "COMIC SHOP LOCATOR",
                    url: '/img/buy-comics-shop-locator.png'
                },
                {
                    name: "DC POWER VISA",
                    url: '/img/buy-dc-power-visa.svg'
                }
            ]
        }
    }
}
</script>

<template>
    <div class="main-content-merchandise">

        <div class="merchandise-content">

            <ul>
                <li v-for="merchandiseLinks in merchandise">
                    <img :src="merchandiseLinks.url" alt="Merchandise Logo">
                    {{ merchandiseLinks.name }}
                </li>
            </ul>

        </div>

    </div>
</template>

<style lang="scss">
@use '../styles/variables' as *;

.main-content-merchandise {
    background-color: $primaryColor;

    .merchandise-content {
        padding-top: 50px;
        padding-bottom: 50px;
        max-width: 1270px;
        margin: auto;

        ul {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 50px;
            list-style-type: none;

            li {
                display: flex;
                justify-content: center;
                align-items: center;
                gap: 10px;

                img {
                    object-fit: contain;
                    width: 50px;
                    height: 50px;
                }
            }
        }
    }
}
</style>