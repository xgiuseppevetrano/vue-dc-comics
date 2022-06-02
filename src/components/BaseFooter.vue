<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="footer-top__link">
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-digital-comics.png" alt="digital Comics">
                        <small>Digital Comics</small>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
                        <small>Dc merchandise</small>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
                        <small>Subscription</small>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-shop-locator.png" alt="comics shop locator">
                        <small>Comics shop locator</small>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-dc-power-visa.svg" alt="dc power pisa">
                        <small>Dc power pisa</small>
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
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>          
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h4>Shop</h4>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="footer-center__col">
                        <h4>Dc</h4>
                        <ul>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="footer-center__col">
                        <h4>Sites</h4>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
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
                        <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
                        <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
                        <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
                        <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                        <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'BaseFooter',
    data() {
        return {
            links: [
                {
                    title: 'Dc comics',
                    text: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    title: 'Shop',
                    text: [
                        'Shop DC',
                        'Collectibles',
                    ]
                },
                {
                    title: 'Dc',
                    text: [
                        'Terms Of Use',
                        'Privacy policy',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us'
                    ]
                },
                {
                    title: 'Sites',
                    text: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ]
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.footer-top {
    background-color: var(--primary-color);
    padding: 2.1875rem;

    &__link {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    &__item {
        display: flex;
        align-items: center;
        color: var(--secondary-color-text);
        text-decoration: none;
        text-transform: uppercase;

        &-img {
            height: 2.5rem;
            margin: 0 .9375rem;
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
        }

        ul li a {
            text-decoration: none;
            color: var(--tertiary-color-text);
            font-size: .875rem;
        }

        ul li a:hover {
            color: var(--primary-color);
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
            cursor: pointer;
        }

        & button:hover {
            background-color: var(--primary-color);
            transition: 0.5s;
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

        & a img {
            margin-right: .9375rem;
        }

        & a:hover {
            opacity: 0.7;
            transition: 0.5s;
        }
    }
}
</style>