<script>

import Logo from './Logo.vue';
import Navbar from './Navbar.vue';
export default {
    data() {
        return {
        }
    },
    components: {
        Logo,
        Navbar
    }
}
</script>

<template>
    <div id="header">

        <div class="container">
            <Logo></Logo>
            <Navbar></Navbar>
        </div>
    </div>
</template>

<style scoped>
#header {
    background-color: white;
    width: 100%;
}
.container {
    align-items: center;
    display: flex;
    height: 120px;
    justify-content: space-between;
}
</style>