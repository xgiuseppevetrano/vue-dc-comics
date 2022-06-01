<template>
    <div class="container">
        <header class="header">
            <div class="header__logo">
                <img src="../assets/img/dc-logo.png"/>
            </div>
            <nav class="header__nav">
                <ul>
                    <li v-for="(link, index) in links" :key="index" :class="{active : link.isActive}"><a :href="link.url">{{link.text}}</a></li>
                </ul>
            </nav>
        </header>
    </div>
</template>

<script>
    export default {
        name: 'BaseHeader',
        data() {
            return {
                links: [
                    {
                        text: "Characters",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "Comics",
                        url: "#",
                        isActive: true,
                    },
                    {
                        text: "Movie",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "Tv",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "Games",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "Collectibles",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "Videos",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "Fans",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "News",
                        url: "#",
                        isActive: false,
                    },
                    {
                        text: "Shop",
                        url: "#",
                        isActive: false,
                    },
                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
    .header {
        position: relative;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1.25rem;

        &__logo {
            img {
                height: 3.75rem;
            }
        }
        &__nav {
            ul {
                display: flex;
                justify-content: center;
                list-style-type: none;
                text-transform: uppercase;
                font-size: .875rem;
                font-weight: 500;
                a {
                    display: inline-block;
                    padding: 1.875rem 1.25rem;
                    text-decoration: none;
                    color: var(--primary-color-text);
                }
                .active a {
                    color: var(--primary-color);
                }
            }
        }
    }
</style>