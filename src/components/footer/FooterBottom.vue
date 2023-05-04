<script>
import LoginSignup from './LoginSignup.vue';
import SoCial from './Social.vue';
export default {
    name: 'FooterBottom',
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

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

#footer-bottom {
    background-color: variables.$dark-color;
    .container{
        align-items: center;
        display: flex;
        justify-content: space-between;
        padding: 2.5rem;
    }
}
</style>