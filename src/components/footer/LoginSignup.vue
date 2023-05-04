<script>

export default {
    name: 'LoginSignup',
}

</script>

<template>
    <a href="">
        <button> Sign-up now! </button>
    </a>
</template>

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

button{
    background-color: transparent;
    border: 2px solid variables.$brand-color;
    color: variables.$main-color;
    cursor: pointer;
    text-transform: uppercase;
    font-size: 1rem;
    padding: 0.6rem;

    &:hover{
        transform: scale(1.1);
    }
}
</style>