<template>
    <section>
        <div class="container py-5">

            <!-- title -->
            <h2 class="fw-bold text-center">Designed for developers</h2>
            <p class="text-center">Build more and spend less time managing your infrastructure with our easy-to-use control panel and API.</p>

            <!-- carousel -->
            <CustomSlider/>

        </div>
    </section>
</template>

<script>
import CustomSlider from '../commons/CustomSlider.vue';

export default {
    name: 'Designe',
    components: {
        CustomSlider
    }
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

section {
    background-color: $sectionColor;
}

</style>