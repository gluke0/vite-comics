<script>
export default {
    name: 'Navbar',
    data() {
        return {
            navbar: [
                {
                    menu: 'Characters',
                    active: false,
                }
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News',
                'Shop'
            ]
        }
    }
}
</script>

<template>
    <div id="navbar">
        <ul>
            <li v-for="item in navbar"><a href="#">{{ item }}</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

ul {
    display: flex;
    text-transform: uppercase;

    li{
        margin-left: 1.25rem;

        a{
            color: variables.$darken-color;
            &.active {
                border-bottom: 0.5rem solid variables.$brand-color;
                color: variables.$brand-color;
            }
        }
    }
}

</style>