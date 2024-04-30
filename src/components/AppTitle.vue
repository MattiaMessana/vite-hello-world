<script>
    export default {
        data () {
            return {
                title: "La mia prima app con Vite! ",
                image: "img01.jpg",
            };
        },
        methods: {
            getImagePath(imageName) {
                return new URL(`../assets/image/${imageName}`, import.meta.url).href;
            },
        },
    };
</script>

<template>
    <h1> {{ title }} </h1>
    <img :src="getImagePath(image)" alt="" />
    
</template>

<style>

</style>
