<script>
export default {
    data() {
        return {
            buttons: [
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'DC Merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    text: 'Subscription'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: 'Comic Shop Locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    text: 'DC Power VISA'
                }
            ]
        }
    }
}
</script>

<template>
    <div id="main-bottom">
        <div class="container">
            <div v-for="button in buttons" class="button">
                <div class="image"></div>
                <div class="text"> {{ button.text }}</div>
            </div>
        </div>
    </div>
</template>

<style scoped>
#main-bottom {
    background-color: rgb(2, 130, 249);
}
.container {
    align-items: center;
    display: flex;
    justify-content: center;
    height: 155px;
}

.button{
    align-items: center;
    color: white;
    display: flex;
    margin: 0 0.8rem;
    text-transform: uppercase;
}

.image{
    aspect-ratio: 1;
    background-color: white;
    margin-right: 0.6rem;
    width: 50px;
}
</style>