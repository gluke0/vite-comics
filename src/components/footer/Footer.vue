<script>
import FooterTop from './FooterTop.vue';
import FooterBottom from './FooterBottom.vue';

export default {
    name: 'Footer',
    components: {
        FooterTop,
        FooterBottom,
        
    }
}
</script>

<template>
    <footer>
        <FooterTop></FooterTop>
        <FooterBottom></FooterBottom>
    </footer>
</template>