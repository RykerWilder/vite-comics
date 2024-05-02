<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<template>

    <footer>
        <div class="container">

            <div class="col">
                <div>
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </div>
                <div>
                    <h2>SHOP</h2>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
            </div>
            <div class="col">
                <h2>DC</h2>
                <ul>
                    <li>Terms Of Use</li>
                    <li>Privacy policy (New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
            </div>
            <div class="col">
                <h2>Sites</h2>
                <ul>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
        </div>
        <div class="ftr-logo"></div>
    </footer>
</template>

<style lang="scss" scoped>

    img {
        max-width: 100%;

    }

    footer {
        gap: 20px;
        display: flex;
        justify-content: space-between;
        font-size: .6rem;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        height: 400px;
    }

    .container {
        padding: 20px;
        width: 30%;
        display: flex;
        justify-content: space-between;
    }

    .col {
        display: flex;
        flex-direction: column;
        gap: 30px;

        h2 {
            color: white;
        }

        ul {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
        }

        li {
            color: grey;
        }
    }

    .ftr-logo {
        width: 70%;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-size: 100%;
        background-position: center;
    }

</style>