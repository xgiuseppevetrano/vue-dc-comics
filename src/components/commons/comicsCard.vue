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
            width: calc(100% / 6 - 1.875rem);
            text-align: left;
            margin: .9375rem;
            
            &-img {
                width: 100%;
                height: 150px;
                object-fit: cover;
                object-position: top;
            }

            &-text {
                color: var(--secondary-color-text);
            }
        }
    }
</style>