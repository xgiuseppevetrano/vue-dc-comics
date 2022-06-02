<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="footer-top__link">
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-digital-comics.png" alt="digital Comics">
                        <span>Digital Comics</span>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
                        <span>Dc merchandise</span>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
                        <span>Subscription</span>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-shop-locator.png" alt="comics shop locator">
                        <span>Comics shop locator</span>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-dc-power-visa.svg" alt="dc power pisa">
                        <span>Dc power pisa</span>
                    </a>
                </div>
            </div>
        </div>
        <div class="footer-center">
            <div class="container">
                <div class="footer-center__row">
                    <div class="footer-center__col">
                        <h4>Dc comics</h4>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h4>Shop</h4>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="footer-center__col">
                        <h4>Dc</h4>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy</li>
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
                    <div class="footer-center__col">
                        <h4>Sites</h4>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="footer-bottom__wrapper">
                    <button>Sign-up now!</button>
                    <div class="footer-bottom__social">
                        <span>Follow us</span>
                        <img src="../assets/img/footer-facebook.png" alt="facebook">
                        <img src="../assets/img/footer-twitter.png" alt="twitter">
                        <img src="../assets/img/footer-youtube.png" alt="youtube">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                        <img src="../assets/img/footer-periscope.png" alt="periscope">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'BaseFooter',
}
</script>

<style lang="scss" scoped>
.footer-top {
    background-color: var(--primary-color);
    padding: 2.1875rem;

    &__link {
        display: flex;
        align-items: center;
        justify-content: space-around;
    }

    &__item {
        display: flex;
        align-items: center;
        color: var(--secondary-color-text);
        text-decoration: none;
        text-transform: uppercase;

        &-img {
            height: 2.5rem;
            margin-right: .9375rem;
        }
    }
}

.footer-center {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    color: var(--secondary-color-text);

    &__row {
        display: flex;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center right;
    }

    &__col {
        width: 10%;
        margin: 0 .625rem;
        padding: 1.875rem 0;

        h4 {
            margin-bottom: .625rem;
            margin-top: .9375rem;
            text-transform: uppercase;
        }

        ul li {
            list-style-type: none;
            font-size: .875rem;
            color: var(--tertiary-color-text);
        }
    }
}

.footer-bottom {
    background-color: var(--tertiary-color);
    padding: 1.5625rem 0;

    &__wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;

        & button {
            padding: .625rem;
            border: .125rem solid var(--primary-color);
            background-color: transparent;
            color: var(--secondary-color-text);
            text-transform: uppercase;
        }
    }

    &__social {
        display: flex;
        align-items: center;

        & span {
            text-transform: uppercase;
            font-weight: 500;
            color: var(--primary-color);
            margin-right: 1.5625rem;
        }

        & img {
            margin-right: .9375rem;
        }
    }
}
</style>