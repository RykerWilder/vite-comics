<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<template>
    <div class="footer-top">
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
            <div class="footer-logo"></div>
        </div>
    </div>

    <div class="footer-bottom">
        <div class="container">
            <div class="container-bottom">
                <button>SIGN-UP NOW</button>
                <div class="socials">
                    <h2>FOLLOW US</h2>
                    <ul>
                        <li><img src="../assets/img/footer-facebook.png" alt=""></li>
                        <li><img src="../assets/img/footer-periscope.png" alt=""></li>
                        <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
                        <li><img src="../assets/img/footer-twitter.png" alt=""></li>
                        <li><img src="../assets/img/footer-youtube.png" alt=""></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

img {
    max-width: 100%;

}

.footer-top {
    font-size: .6rem;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    height: 300px;

    .container {
        height: 100%;
        display: flex;
        justify-content: space-evenly;
        gap: 50px;
    }
}

.col {
    display: flex;
    flex-direction: column;
    padding: 20px 0;

    h2 {
        font-size: 1.3rem;
        color: white;
    }

    ul {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: space-evenly;

        li {
            font-size: .9rem;
            color: grey;
            list-style-type: none;
        }
    }

}

.footer-logo {
    width: 70%;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-size: 100%;
    background-position: center;
}

.footer-bottom {
    display: flex;
    justify-content: space-between;
    background-color: $footer_color;
    padding: 20px 20px;

    .container-bottom {
        display: flex;
        justify-content: space-between;
    }

    button {
        color: white;
        padding: 10px;
        border: 3px solid $primary_color;
        background-color: $footer_color;
        transition: background-color .6s linear;

        &:hover {
            background-color: $primary_color;
        }
    }

    .socials {
        display: flex;
        align-items: center;
        gap: 30px;

        h2 {
            color: $primary_color;
        }

        ul {
            display: flex;
            justify-content: space-between;
            gap: 10px;

            li {
                list-style-type: none;

                img {
                    transition: transform .6s linear;
                    &:hover {
                        transform: scale(1.2);
                    }
                }
            }
        }
    }
}
</style>