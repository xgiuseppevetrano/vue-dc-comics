<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="footer-top__link">
                    <a v-for="(shopLink, index) in shopLinks" :key="index" href="#" class="footer-top__item">
                        <img class="footer-top__item-img" :src="require(`../assets/img/${shopLink.src}`)" :alt="shopLink.name">
                        <small>{{shopLink.name}}</small>
                    </a>
                </div>
            </div>
        </div>
        <div class="footer-center">
            <div class="container">
                <div class="footer-center__row">
                    <div class="footer-center__col" v-for="(link, index) in links" :key="index">
                        <h4 class="footer-center__col-title">{{link.title}}</h4>
                        <ul>
                            <li class="footer-center__col-item" v-for="(text, index) in link.texts" :key="index">
                                <a class="footer-center__col-link" href="#">{{text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="footer-bottom__wrapper">
                    <button class="footer-bottom__button">Sign-up now!</button>
                    <div class="footer-bottom__social">
                        <span class="footer-bottom__social-text">Follow us</span>
                        <a v-for="(social, index) in socials" :key="index" class="footer-bottom__social-link" href="#">
                            <img class="footer-bottom__social-img" :src="require(`../assets/img/${social.src}`)" :alt="social.name">
                        </a>
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
            shopLinks: [
                {
                    name: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    name: 'Dc merchandise',
                    src: 'buy-comics-merchandise.png'
                },
                {
                    name: 'Subscription',
                    src: 'buy-comics-subscriptions.png'
                },
                {
                    name: 'Comics shop locator',
                    src: 'buy-comics-shop-locator.png'
                },
                {
                    name: 'Dc power pisa',
                    src: 'buy-dc-power-visa.svg'
                }
    
            ],
            links: [
                {
                    title: 'Dc comics',
                    texts: [
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
                    texts: [
                        'Shop DC',
                        'Collectibles',
                    ]
                },
                {
                    title: 'Dc',
                    texts: [
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
                    texts: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ]
                }
            ],
            socials: [
                {
                    name: 'facebook',
                    src: 'footer-facebook.png'
                },
                {
                    name: 'twitter',
                    src: 'footer-twitter.png'
                },
                {
                    name: 'youtube',
                    src: 'footer-youtube.png'
                },
                {
                    name: 'pinterest',
                    src: 'footer-pinterest.png'
                },
                {
                    name: 'periscope',
                    src: 'footer-periscope.png'
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
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    color: var(--secondary-color-text);

    &__row {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        align-content: flex-start;
        height: 350px;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center right;
    }

    &__col {
        width: 10%;
        margin: 0 .625rem;
        padding: 0.775rem 0;

        &-title {
            margin-bottom: .625rem;
            margin-top: .9375rem;
            text-transform: uppercase;
        }

        &-item {
            list-style-type: none;
        }

        &-link{
            text-decoration: none;
            color: var(--tertiary-color-text);
            font-size: .875rem;
        }

        &-link:hover {
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
    }

    &__button {
        padding: .625rem;
        border: .125rem solid var(--primary-color);
        background-color: transparent;
        color: var(--secondary-color-text);
        text-transform: uppercase;
        cursor: pointer;
    }

    &__button:hover {
        background-color: var(--primary-color);
        transition: 0.5s;
    }

    &__social {
        display: flex;
        align-items: center;

        &-text {
            text-transform: uppercase;
            font-weight: 500;
            color: var(--primary-color);
            margin-right: 1.5625rem;
            cursor: pointer;
        }

        &-link:hover {
            opacity: 0.7;
            transition: 0.5s;
        }

        &-img {
            margin-right: .9375rem;
        }
    }
}
</style>