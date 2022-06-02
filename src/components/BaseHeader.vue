<template>
    <header>
        <div class="container">
            <div class="header">
                <div class="header__logo">
                    <img src="../assets/img/dc-logo.png"/>
                </div>
                <nav class="header__nav">
                    <ul>
                        <li v-for="(link, index) in links" :key="index" :class="{active : link.isActive}" @click="navActive(index)"><a :href="link.href">{{link.text}}</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        name: 'BaseHeader',
        data() {
            return {
                links: [
                    {
                        text: "Characters",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Comics",
                        href: "#",
                        isActive: true,
                    },
                    {
                        text: "Movie",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Tv",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Games",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Collectibles",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Videos",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Fans",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "News",
                        href: "#",
                        isActive: false,
                    },
                    {
                        text: "Shop",
                        href: "#",
                        isActive: false,
                    },
                ],
            }
        },
        methods: {
            navActive(index) {
                this.links[index].isActive = !this.links[index].isActive;
            }
        }
    }
</script>

<style lang="scss" scoped>
    header {
        position: relative;

        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            &__logo {
                img {
                    height: 4.375rem;
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
                        padding: 2.1875rem 0;
                        text-decoration: none;
                        color: var(--primary-color-text);
                        border-bottom: .3125rem solid transparent;
                        margin: 0 .9375rem;
                    }
                    .active a {
                        color: var(--primary-color);
                        border-color: var(--primary-color);
                    }
                    a:hover {
                        color: var(--primary-color);
                        border-color: var(--primary-color);
                    }
                }
            }
        }
    }
</style>