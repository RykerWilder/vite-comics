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
            console.log(imageName);
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
                    <div class="img-container">
                        <img :src="getImageUrl(icon.path)" alt="">
                    </div>
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

                .img-container {
                    width: 30%;

                    img {
                        max-width: 100%;
                    }
                }

                h4 {
                    color: white;
                    font-size: .5rem;
                }
            }
        }
    }

</style>