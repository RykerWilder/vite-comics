<script>
import AppCard from './AppCard.vue';
export default {

    components : {
        AppCard
    }
}
</script>

<template>

    <main>
        <section class="series">
            <button class="btn-series">CURRENT SERIES</button>
            <div class="container">
                <div class="row">
                    <div class="col" v-for="item in series">
                        <AppCard />
                    </div>
                </div>
                <button id="load">LOAD MORE</button>
            </div>

        </section>

    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

main {
    height: 100%;
    width: 100%;
    color: white;

    .series {
        padding: 20px;
        background-color: black;

        .btn-series {
            padding: 10px 16px;
            border: 0;
            background-color: $primary_color;
            color: white;
            font-size: 1.6rem;
            font-weight: bold;
            position: relative;
            left: 150px;
            top: -40px;
        }

        .row {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }
    
        .col {
            width: calc(100% / 5);
            padding: 40px;
        }

        #load {
            cursor: pointer;
            display: block;
            padding: 10px 55px;
            margin: 0 auto;
            background-color: $primary_color;
            border: 0;
            color: white;
            transition: transform .6s linear;

            &:hover {
                transform: scale(1.2);
            }
        }
    }


}
</style>