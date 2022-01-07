<template>
    <Carousel>
        <Slide>
            contenuto
        </Slide>
        <Slide>
            contenuto
        </Slide>
    </Carousel>
</template>

<script>

import { Carousel, Slide } from 'vue-carousel';

export default {
    name: 'CustomSlider',
    components: {
        Carousel,
        Slide
    }
}
</script>

<style lang='scss' scoped>

</style>