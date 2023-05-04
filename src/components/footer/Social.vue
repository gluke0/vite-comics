<script>
export default {
    name: 'SoCial',
    data() {
        return {
            socials:[
                {
                    social: 'Facebook',
                    logo: 'footer-facebook.png'
                },
                {
                    social: 'Twitter',
                    logo: 'footer-twitter.png'
                },
                {
                    social: 'YouTube',
                    logo: 'footer-YouTube.png'
                },
                {
                    social: 'Pinterest',
                    logo: 'footer-pinterest.png'
                },
                {
                    social: 'Periscope',
                    logo: 'footer-periscope.png'
                },
            ]
        }
    },
    methods:{
        getImagePath: function (imgPath){
            return new URL(imgPath, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div id="socials">
        <h3> Follow us </h3>
        <div class="buttons">
            <div v-for="social in socials" class="button">
                <a href="#">
                    <img :src="getImagePath(`../../../public/img/${social.logo}`)" :alt="social.social">
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

#socials{
    align-items: center;
    display: flex;

    h3{
        margin-right: 1rem;
        color: variables.$brand-color;
        text-transform: uppercase;
    }
    .buttons{
        display: flex;

        .button{
            margin-left: 1rem;
            width: 2rem;

            &:hover{
                transform: scale(1.1);
            }
        }
    }
    
}

</style>