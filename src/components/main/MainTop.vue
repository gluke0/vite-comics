<script>
export default {
    name: 'MainTop'
}
</script>

<template>
    <div id="main-top">
        <div class="container">
            --&gt; <strong> Content goes here </strong> &lt;--
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../../public/style/partials/variables';

    #main-top{
        background-color: variables.$darken-color;

        .container {
            align-items: center;
            color: variables.$main-color;
            display: flex;
            font-size: 2rem;
            padding: 4rem 0;
        }
    }   
</style>
