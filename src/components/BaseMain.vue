<template>
    <main>
        <div class="container">
            <p>Content goes here</p>
        </div>
    </main>
</template>

<script>
export default {
    name: 'BaseMain',
}
</script>

<style lang="scss" scoped>
    main {
        background-color: var(--secondary-color);
        padding: 2.5rem;
        text-align: center;
        color: var(--secondary-color-text);
        font-weight: 500;
    }
</style>