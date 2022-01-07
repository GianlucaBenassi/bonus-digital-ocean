<template>
    <section>
        <div class="container py-5">

            <!-- title -->
            <h2 class="text-center fw-bold">Deploy and scale seamlessly</h2>
            <p class="text-center">Our optimized configuration process saves your team time when running ans scaling distributed applications, AI & machine learning workloads, hosted services, client websites, or CI/CD environments.</p>

            <div class="row mt-5">

                <!-- list column -->
                <div class="col-12 col-md-2 mb-2 mb-md-0">
                    <ul class="ps-0">
                        <li class="border-start ps-2 py-1">Deploy</li>
                        <li class="border-start ps-2 py-1">Manage</li>
                        <li class="border-start ps-2 py-1">Secure</li>
                        <li class="border-start ps-2 py-1">Scale</li>
                        <li class="border-start ps-2 py-1">Monitor</li>
                    </ul>
                </div>

                <!-- description column-->
                <div class="col-12 col-md-10">
                    <div class="row row-cols-1 row-cols-md-2">

                        <div class="col" v-for="(card, index) in cards" :key="index">
                            <Card :infos="card"/>
                        </div>
                        
                    </div>
                </div>

            </div>

        </div>
    </section>
</template>

<script>

import Card from '../commons/Card.vue';

export default {
    name: 'Deploy',
    components: {
        Card
    },
    data() {
        return {
            cards: [
                {
                    img: require('../../assets/img/cluster-deploy.svg'),
                    title: 'Cluster deployments',
                    desc: 'Provision multiple Droplets (virtual machines) in seconds with our control panel, CLI, or directly against our API.'
                },
                {
                    img: require('../../assets/img/optimized-compute.svg'),
                    title: 'Optimized compute types',
                    desc: 'Get the compute resources you need with Standard or Optimized Droplets.'
                },
                {
                    img: require('../../assets/img/one-click.svg'),
                    title: 'One-click apps',
                    desc: 'Skip the install and configuration process with pre-build open source images supporting Rails, Cassandra, Docker, and more.'
                },
                {
                    img: require('../../assets/img/global.svg'),
                    title: 'Global availability',
                    desc: 'Deploy to any of our data center regions around the world.'
                }
            ]
        }
    }
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

li {
    color: $textColor;
}

</style>