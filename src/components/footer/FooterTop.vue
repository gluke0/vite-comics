<script>
import FooterList from './FooterList.vue';
export default {
    data() {
        return {
        }
    },
    components:{
        FooterList
    }
}
</script>

<template>
    <div id="footer-top">
        <div class="container">
            <div class="left column">
                <FooterList></FooterList>
                <FooterList></FooterList>
            </div>
            <div class="center column">
                <FooterList></FooterList>
            </div>
            <div class="right column">
                <FooterList></FooterList>
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
.column {
    margin: 2rem 1.3rem 2rem 0;
}
</style>