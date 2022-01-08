<template>
    <Carousel 
    :per-page="1"
    :navigationEnabled="navigation"
    :navigationPrevLabel='`<i class="fas fa-chevron-left fs-1"></i>`'
    :navigationNextLabel='`<i class="fas fa-chevron-right fs-1"></i>`'
    >
        <Slide v-for="(info, index) in infos" :key="index">

            <img class="w-100" :src="info.image" :alt="'slide image ' + index">
            <p class="text-center mt-3">{{info.desc}}</p>
            <span v-if="info.author" class="d-block text-center fw-bold">{{info.author.name}}</span>
            <span v-if="info.author" class="d-block text-center">{{info.author.role}}</span>
            <a href="#" v-if="info.story" class="d-block text-center mt-3 pb-5">{{info.story}} &gt;</a>

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
    },
    props: {
        infos: Array
    },
    data() {
        return {
            navigation: true
        }
    },
    methods: {
        OnResize() {
            if (window.innerWidth < 768) {
                this.navigation = false;
            } else {
                this.navigation = true;
            }
        }
    },
    mounted() {
        this.OnResize();
        window.addEventListener('resize', this.OnResize, {passive: true});
    }
}
</script>

<style lang='scss'>

@import '../../assets/style/variables.scss';

.VueCarousel {
    width: 80%;

    .VueCarousel-dot {
        border: 1px solid $mainColor;
        padding: 0 !important;
        margin: 0 5px;

        &--active{
            background-color: $mainColor !important;
        }
    }

    &.teams_carousel {
        .VueCarousel-wrapper {
            background-color: #fff;
            border-radius: .25rem;
        }
    }
}

</style>