<template>
    <section>
        
        <div class="container py-5">
            
            <h2 class="text-center fw-bold mb-5">The features your business needs</h2>

            <div class="row row-cols-1 row-cols-md-3">
                
                <div class="col mb-3 mb-md-0" v-for="(card, index) in cards" :key="index">
                    <Card :infos="card"/>
                </div>
                

            </div>

        </div>

    </section>
</template>

<script>
import Card from '../commons/Card.vue';

export default {
    name: 'Features',
    components: {
        Card
    },
    data() {
        return {
            cards: [
                {
                    img: require('../../assets/img/pred-pricing.svg'),
                    title: 'Predictable pricing',
                    desc: 'Leave complex pricing structures behind. Always know what you\'ll pay per month with a flat, industry-leading pricing structure.',
                    link: 'Pricing'
                },
                {
                    img: require('../../assets/img/world-class.svg'),
                    title: 'World-class service',
                    desc: 'Free round-the-clock techical support for all customers. You\'ll feel the love.',
                    link: 'Support'
                },
                {
                    img: require('../../assets/img/reliable-platform.svg'),
                    title: 'Reliable platform',
                    desc: 'More than 100,000 developers teams worldwide trust DigitalOcean to support ther business with a 99.99%  uptime SLA for all services.',
                    link: 'Security'
                }
            ]
        }
    }
}
</script>

<style lang='scss' scoped>

</style>