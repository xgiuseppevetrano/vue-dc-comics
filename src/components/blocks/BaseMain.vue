<template>
    <main>
        <SectionJumbotron/>
        <SectionCards/>
    </main>
</template>

<script>
import SectionCards from "../sections/sectionCards.vue";
import SectionJumbotron from "../sections/sectionJumbotron.vue";

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