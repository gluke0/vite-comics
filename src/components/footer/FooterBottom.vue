<script>
import LoginSignup from './LoginSignup.vue';
import SoCial from './Social.vue';
export default {
    data() {
        return {
        }
    },
    components: {
        LoginSignup,
        SoCial,
    }
}
</script>

<template>
    <div id="footer-bottom">
        <div class="container">
            <LoginSignup> </LoginSignup>
            <SoCial> </SoCial>
        </div>
    </div>
</template>

<style scoped>
#footer-bottom {
    background-color: rgb(48, 48, 48);
}
.container {
    align-items: center;
    display: flex;
    height: 100px;
    justify-content: space-between;
}
</style>