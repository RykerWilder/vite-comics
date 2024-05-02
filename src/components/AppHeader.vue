<script>
export default {
    data() {
        return {
            menu: [
                {
                    option: 'CHARACTERS',
                    isActive: false
                },
                {
                    option: 'COMICS',
                    isActive: false
                },
                {
                    option: 'MOVIES',
                    isActive: false
                },
                {
                    option: 'TV',
                    isActive: false
                },
                {
                    option: 'GAMES',
                    isActive: false
                },
                {
                    option: 'COLLECTIBLES',
                    isActive: false
                },
                {
                    option: 'VIDEOS',
                    isActive: false
                },
                {
                    option: 'FANS',
                    isActive: true
                },
                {
                    option: 'NEWS',
                    isActive: false
                },
                {
                    option: 'SHOP',
                    isActive: false
                }
            ]
        }
    }
}
</script>

<template>

    <header>
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo DC">
        </div>
        <div class="menu">
            <ul>
                <li v-for="item in menu" :class="{ active: item.isActive }"> {{ item.option }} </li>
            </ul>
        </div>

    </header>
</template>

<style lang="scss">

    @use "../style/partials/variables" as *;

    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

    img {
        display: block;
        max-width: 100%;
    }

    header {
        padding: 0 20px;
        height: 150px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .menu {
        height: 100%;
    }

    ul {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 10px;
    }

    li {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;
        list-style-type: none;
    }

    .active {
        border-bottom: 5px solid $primary_color;
        color: $primary_color;
    }
</style>