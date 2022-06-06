<template>
    <main>
        <SectionJumbotron/>
        <SectionCards/>
    </main>
</template>

<script>
import SectionCards from "../sections/SectionCards.vue";
import SectionJumbotron from "../sections/SectionJumbotron.vue";

export default {
    name: 'BaseMain',
    components: {
        SectionCards,
        SectionJumbotron
    }
}
</script>

<style lang="scss" scoped>

</style>