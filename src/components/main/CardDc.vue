<script>
export default {
    name: 'CardDc',
    props: {
        img: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <div class="image">
            <img :src="img" :alt="title">
        </div>
        <h3 class="title">{{ title }}</h3>
    </div>
</template>

<style scoped>

.image {
    aspect-ratio: 1;
    width: 50%;
    display: flex;
    justify-content: center;
    width: fit-content;
}

.image img{
    height: 200px;
    width: 200px;
}

.title{
    text-transform: uppercase;
    font-size: 0.8rem;
    margin-top: 0.9rem;
}
</style>