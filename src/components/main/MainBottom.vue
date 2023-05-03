<script>
import Shop from './Shop.vue';
export default {
    data() {
        return {
        }
    },
    components: {
        Shop
    }
}
</script>

<template>
    <div id="main-bottom">
        <div class="container">
            <Shop></Shop>
            <Shop></Shop>
            <Shop></Shop>
            <Shop></Shop>
            <Shop></Shop>
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
</style>