<script>
export default {
    name: "AppNav",

    data() {
        return {
            links: ["Characters", "Comics", "Movies", "Tv", "Games", "Collectibles", "Videos", "Fans", "News", "Shop"],

            activeLinkIndex: 1,
        }
    }
}
</script>

<template>
    <nav>

        <div class="nav-content">

            <div class="logo">
                <img src="/img/dc-logo.png" alt="DC logo">
            </div>

            <div class="nav-links">

                <ul>
                    <li v-for="activeLinks in links">
                        {{ activeLinks }}
                    </li>
                </ul>

            </div>

        </div>

    </nav>
</template>

<style lang="scss">
nav {
    background-color: white;
    color: black;

    .nav-content {
        display: flex;
        max-width: 1270px;
    }

    .logo img {
        width: 75px;
        height: 75px;
    }

    .nav-links {
        ul {
            list-style-type: none;
            display: flex;
        }
    }
}
</style>
