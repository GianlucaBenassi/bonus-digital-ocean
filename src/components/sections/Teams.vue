<template>
    <section>
        <div class="container py-5">

            <h2 class="text-center fw-bold mb-5">Development teams love DigitalOcean</h2>

            <CustomSlider :infos="slides" class="mx-auto teams_carousel"/>

        </div>
    </section>
</template>

<script>

import CustomSlider from '../commons/CustomSlider.vue';

export default {
    name: 'Teams',
    components: {
        CustomSlider
    },
    data() {
        return {
            slides: [
                {
                    image: require('../../assets/img/rockerbox.png'),
                    desc: '"We have been able to make scaling the technical infrastructure of our business cost effective and efficient."',
                    author: {
                        name: 'Rick O\'Toole',
                        role: 'Co-founder and CTO'
                    },
                    story: 'Read story'
                },
                {
                    image: require('../../assets/img/rockerbox.png'),
                    desc: '"We have been able to make scaling the technical infrastructure of our business cost effective and efficient."',
                    author: {
                        name: 'Rick O\'Toole',
                        role: 'Co-founder and CTO'
                    },
                    story: 'Read story'
                },
                {
                    image: require('../../assets/img/rockerbox.png'),
                    desc: '"We have been able to make scaling the technical infrastructure of our business cost effective and efficient."',
                    author: {
                        name: 'Rick O\'Toole',
                        role: 'Co-founder and CTO'
                    },
                    story: 'Read story'
                }
            ]
        }
    }
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

section {
    background-color: $sectionColor;

    .VueCarousel-wrapper {
        background-color: #fff;
    }
}

</style>