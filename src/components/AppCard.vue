<script>
    export default {
        props: {
            serie: Object
        },
        data() {
            return {

            }
        }
    }
</script>

<template>

<div class="card">
        <img :src="serie.thumb" alt="">
        <h4>{{ serie.series }}</h4>
    </div>

</template>

<style lang="scss" scoped>

.card {
    height: 300px;

    img {
        object-fit: contain;
        height: 80%;
        display: block;
        margin-bottom: 10px;
    }
}

</style>
