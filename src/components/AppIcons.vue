<script>
export default {
    data() {
        return {
            banner: [
                {
                    path: "comics-digital-comics.png",
                    name: "DIGITAL COMICS",
                },
                {
                    path: "comics-merchandise.png",
                    name: "DC MERCHANDISE",
                },
                {
                    path: "comics-subscriptions.png",
                    name: "SUBSCRIPTION",
                },
                {
                    path: "comics-shop-locator.png",
                    name: "COMIC SHOP LOCATOR",
                },
                {
                    path: "dc-power-visa.svg",
                    name: "DC POWER VISA",
                },

            ],
        }
    },
    methods: {
        getImageUrl(imageName) {
            return new URL(`../assets/img/buy-${imageName}`, import.meta.url).href;
        }
    }
}
</script>

<template>

    <div>
        <div class="container">
            <ul>
                <li v-for="icon in banner">
                    <img :src="getImageUrl(icon.path)" alt="">
                    <h4>{{ icon.name }}</h4>
                </li>
            </ul>
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

div {
    background-color: $primary_color;

    ul {
        display: flex;
        justify-content: space-between;
        align-items: center;

        li {
            padding: 20px;
            width: calc(100% / 5);
            list-style-type: none;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 30px;

            img {
                height: 70px;
                transition: transform .6s linear;

                &:hover {
                    transform: scale(1.2);
                }
            }

            h4 {
                padding: 10px;
                width: 70%;
                color: white;
                font-size: .8rem;
            }
        }
    }
}
</style>