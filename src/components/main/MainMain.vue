<script>
import MainTop from './MainTop.vue';
import MainBottom from './MainBottom.vue';

export default {
    name: 'MainMain',
    components: {
        MainTop,
        MainBottom,
    }
}
</script>

<template>
    <main>
        <MainTop> </MainTop>
        <MainBottom> </MainBottom>
    </main>
</template>