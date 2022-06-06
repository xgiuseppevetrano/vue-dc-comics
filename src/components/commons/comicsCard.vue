<template>
    <div class="comics__card">
        <img class="comics__card-img" :src="thumb" :alt="series">
        <small class="comics__card-text">{{series}}</small>
    </div>
</template>

<script>
export default {
    name: 'ComicsCard',
    props: {
        thumb: String,
        series: String
    }
}
</script>

<style lang="scss" scoped>
    .comics {
        &__card {
            width: calc(100% / 6 - 2.5rem);
            text-align: left;
            margin: .9375rem;
            &-img {
                width: 100%;
            }

            &-text {
                color: var(--secondary-color-text);
            }
        }
    }
</style>