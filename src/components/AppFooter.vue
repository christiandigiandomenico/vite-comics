<script>
export default {
    name: "AppFooter",

    data() {
        return {
            links: [
                {
                    title: "DC COMICS",
                    list: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News"
                    ]
                },
                {
                    title: "SHOP",
                    list: [
                        "Shop DC",
                        "Shop DC Collectibles"
                    ]
                },
                {
                    title: "DC",
                    list: [
                        "Terms of use",
                        "Privacy policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPCS Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact Us"
                    ]
                },
                {
                    title: "SITES",
                    list: [
                        "DC",
                        "MAD Magazines",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa",
                    ]
                }
            ]
        }
    }
}
</script>

<template>
    <div class="navbar-links">

        <div class="links">
            <div v-for="linkList in links" class="links-list">
                <h3>{{ linkList.title }}</h3>
                <ul>
                    <li v-for="currentLink in linkList.list">
                        {{ currentLink }}
                    </li>
                </ul>
            </div>
        </div>

        <img src="/img/dc-logo-bg.png" alt="DC Logo">

    </div>
    <div class="footer-information-container">
        <div class="footer-information">

            <button>SIGN-UP NOW!</button>

            <div class="follow-us">

                <span>FOLLOW US</span>

                <img src="/img/footer-facebook.png" alt="Facebook">
                <img src="/img/footer-twitter.png" alt="Twitter">
                <img src="/img/footer-youtube.png" alt="Youtube">
                <img src="/img/footer-pinterest.png" alt="Pinterest">
                <img src="/img/footer-periscope.png" alt="Periscope">


            </div>

        </div>
    </div>
</template>

<style lang="scss">
.navbar-links {
    background-image: url(/img/footer-bg.jpg);
    background-size: cover;
    position: relative;

    img {
        position: absolute;
        right: 100px;
        bottom: -70px;
        z-index: 1;
    }
}

.links {
    max-width: 1270px;
    margin: auto;
    display: flex;
    gap: 20px;
    padding: 40px;

    .links-list {

        ul {
            list-style-type: none;
            text-align: start;
            padding-left: 0;

            li {
                text-align: start;
            }
        }
    }
}

.footer-information-container {
    background-color: #303030;
    z-index: 99;
    position: relative;
}

.footer-information {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1270px;
    margin: auto;
    padding: 20px;
    z-index: 99;

    button {
        border: 1px solid #0282f9;
        background-color: transparent;
        padding: 15px 20px;
    }

    .follow-us {
        display: flex;
        justify-content: center;
        align-items: center;

        span {
            font-size: 20px;
            color: #0282f9;
            font-weight: bold;
        }

        img {
            margin-left: 20px;
        }
    }
}
</style>
