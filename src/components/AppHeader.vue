<script>
export default {
    data() {
        return {
            menu: [
                {
                    option: CHARACTERS,
                    isActive: false
                },
                {
                    option: COMICS,
                    isActive: false
                },
                {
                    option: MOVIES,
                    isActive: false
                },
                {
                    option: TV,
                    isActive: false
                },
                {
                    option: GAMES,
                    isActive: false
                },
                {
                    option: COLLECTIBLES,
                    isActive: false
                },
                {
                    option: VIDEOS,
                    isActive: false
                },
                {
                    option: FANS,
                    isActive: false
                },
                {
                    option: NEWS,
                    isActive: false
                },
                {
                    option: SHOP,
                    isActive: false
                }
            ]
        }
    }
}
</script>

<template>
    <div class="logo"></div>
    <div>
        <ul>
            <li v-for="option in menu"><a href=""></a></li>
        </ul>
    </div>
</template>

<style scoped>

</style>