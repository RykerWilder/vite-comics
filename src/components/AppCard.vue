<script>
import axios from 'axios';

    export default {
        data() {
            return {
                apiKey: 'eec8579b20825f26f241f73e50237f36',
                movies: []
            }
        },
        methods: {
            getFilm() {
                let response = axios.get(`https://api.themoviedb.org/3/collection/172712?api_key=${this.apiKey}`).then(response => {
                    console.log(response.data);
                })
            }                
        },
        mounted() {
            this.getFilm()
        }
    }
</script>

<template>

    <div class="card">
        <img src="" alt="">
        <h4></h4>
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
