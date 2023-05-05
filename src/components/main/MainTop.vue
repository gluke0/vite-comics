<script>
import CardDc from './CardDc.vue';

export default {
    name: 'MainTop',
    components:{
        CardDc
    },
    data (){
        return{
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    }
}       
</script>

<template>
    <div id="main-top">
        <div class="container">
            <h2 class="loadmore" id="currents">Current Series</h2>
            <div class="comics">
                <CardDc v-for="comic in comics"
                class="comic"
                :img="comic.thumb"
                :title="comic.series"></CardDc>
            </div>
            <button class="loadmore"> Load More </button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

    #main-top{
        background-color: variables.$darken-color;

        .container {
            color: variables.$main-color;
            font-size: 2rem;
            padding: 4rem 0;
            display: flex;
            flex-wrap: wrap;

            .comics{
                display: flex;
                justify-content: center;
                flex-wrap: wrap;

                .comic{
                    margin: 0.5rem;
                    width: 12rem;
                }
            }
        }
    }   

    .loadmore{
                margin: 2.5rem auto 0;
                color: variables.$main-color;
                background-color: variables.$brand-color;
                border: none;
                text-transform: uppercase;
                padding: 0.7rem 1.6rem;
            }

            #currents{
                position: absolute;
                font-size: 1.8rem;
                margin: 0;
            }

</style>
