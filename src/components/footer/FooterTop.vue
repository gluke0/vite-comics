<script>

export default {
    name: 'FooterTop',
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

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';
#footer-top{
    background: url(../../../public/img/dc-logo-bg.png) center right 20% no-repeat, url(../../../public/img/footer-bg.jpg) left top no-repeat;
    background-size: auto, cover;
    .container {
        display: flex;
        padding: 2rem 0;
        .column{
            margin: 2rem 1.3rem 2rem 0;

        ul{
            margin: 0.8rem 0;

            li{
                margin: 0.5rem 0;
            
                a{
                    color: variables.$darken-text-color;
                }
            }
        }
        
        h3{
            color: variables.$main-color;
            text-transform: uppercase;
        }
        }
    }
}

</style>