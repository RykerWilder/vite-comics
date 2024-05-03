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
                    isActive: true
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
                    isActive: false
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
        <div class="container header-container">

            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo DC">
            </div>
            <div class="menu">
                <ul>
                    <li v-for="item in menu" :class="{ active: item.isActive }"> {{ item.option }} </li>
                </ul>
            </div>
        </div>

    </header>
</template>

<style lang="scss" scoped>

    @use '../style/partials/variables' as *;

    img {
        display: block;
        max-width: 100%;
    }

    header {
        padding: 0 20px;
        height: 150px;
    }

    .header-container {
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
        line-height: 150px;
        display: flex;
        justify-content: center;
        align-items: center;
        list-style-type: none;
    }

    .active {
        border-bottom: 4px solid $primary_color;
        color: $primary_color;
    }
</style>