<script>

export default {
    data() {
        return {
            comics: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],

            shop: [
                "Shop DC",
                "Shop DC Collectibles"
            ],

            dc: [
                "Terms Of Use",
                "Privacy policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshops",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us"
            ],

            sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ],
        }
    }
}
</script>

<template>
    <div id="footer-top">
        <div class="container">
            <div class="left column">
                <h3>DC Comics</h3>
                <ul>
                    <li v-for="comic in comics"><a href="#">{{ comic }}</a></li>
                </ul>

                <h3>Shop</h3>
                <ul>
                    <li v-for="shop in shop"><a href="#">{{ shop }}</a></li>
                </ul>
            </div>
            <div class="center column">
                <h3>DC</h3>
                <ul>
                    <li v-for="dc in dc"><a href="#">{{ dc }}</a></li>
                </ul>
            </div>
            <div class="right column">
                <h3>Sites</h3>
                <ul>
                    <li v-for="site in sites"><a href="#">{{ site }}</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
#footer-top {
    background-color: rgb(28, 28, 28);
}
.container {
    display: flex;
}
.column{
    margin: 2rem 1.3rem 2rem 0;
}

ul{
    margin: 0.8rem 0;
    color: rgb(124, 126, 128);
}
h3{
    color: white;
}

</style>