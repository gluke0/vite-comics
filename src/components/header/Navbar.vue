<script>
export default {
    name: 'Navbar',
    data() {
        return {
            navbar: [
                {
                    menu: 'Characters',
                    active: false,
                },
                {
                    menu: 'Comics',
                    active: true,
                },
                {
                    menu: 'Movies',
                    active: false,
                },
                {
                    menu: 'TV',
                    active: false,
                },
                {
                    menu: 'Games',
                    active: false,
                },
                {
                    menu: 'Collectibles',
                    active: false,
                },
                {
                    menu: 'Videos',
                    active: false,
                },
                {
                    menu: 'Fans',
                    active: false,
                },
                {
                    menu: 'News',
                    active: false,
                },
                {
                    menu: 'Shop',
                    active: false,
                },
            ]
        }
    }
}
</script>

<template>
    <div id="navbar">
        <ul>
            <li v-for="item in navbar"><a href="#" :class="{active: item.active == true}">{{ item.menu }}</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

ul {
    display: flex;
    text-transform: uppercase;
    align-items: center;

    li{
        margin-left: 1.80rem;

        a{
            color: variables.$darken-color;
            border-bottom: variables.$navbar-border solid transparent;
            display: inline-block;
            line-height: 8rem;
            &.active,
            &:hover{
                border-bottom: 0.5rem solid variables.$brand-color;
                color: variables.$brand-color;
            }
        }
    }
}

</style>