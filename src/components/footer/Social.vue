<script>
import SocialButton from './SocialButton.vue';
export default {
    data() {
        return {
        }
    },
    components: {
        SocialButton
    }
}
</script>

<template>
    <div id="socials">
        <h3> Follow us </h3>
        <div class="buttons">
            <SocialButton></SocialButton>
            <SocialButton></SocialButton>
            <SocialButton></SocialButton>
            <SocialButton></SocialButton>
            <SocialButton></SocialButton>
        </div>
    </div>
</template>

<style scoped>
#socials{
    align-items: center;
    display: flex;
}
h3{
    margin-right: 1.5rem;
}
.buttons{
    display: flex;
}
</style>