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
        <img src="../assets/img/dc-logo.png" alt="logo DC">
        <ul>
            <li v-for="item in menu" :class="{ active: item.isActive }"> {{ item.option }} </li>
        </ul>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.active {
    border-bottom: 4px solid $primary_color;
    color: $primary_color;
}

header {
    z-index: 9999;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100px;
    background-color: white;

    img {
        max-height: 100%;
        padding: 10px;
    }

    ul {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 10px;

        li {
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            list-style-type: none;
        }
    }
}
</style>