<script>

import Logo from './Logo.vue';
import Navbar from './Navbar.vue';

export default {
    name: "HeaderMain",
    components: {
        Logo,
        Navbar
    }
}
</script>

<template>
    <header>
        <div class="container">

            <Logo> </Logo>
            <Navbar> </Navbar>

        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

header{
    background-color: variables.$main-color;
    .container {
        align-items: center;
        display: flex;
        justify-content: space-between;
        }
}
</style>