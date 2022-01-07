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
                    <div class="row">

                        <div class="col-12 col-md-6">
                            <img src="../../assets/img/cluster-deploy.svg" alt="Cluster deployments">
                            <h4 class="fw-bold mt-2">Cluster deployments</h4>
                            <p>Provision multiple Droplets (virtual machines) in seconds with our control panel, CLI, or directly against our API.</p>
                        </div>

                        <div class="col-12 col-md-6">
                            <img src="../../assets/img/optimized-compute.svg" alt="Optimized compute">
                            <h4 class="fw-bold mt-2">Optimized compute types</h4>
                            <p>Get the compute resources you need with Standard or Optimized Droplets.</p>
                        </div>

                        <div class="col-12 col-md-6">
                            <img src="../../assets/img/one-click.svg" alt="One click apps">
                            <h4 class="fw-bold mt-2">One-click apps</h4>
                            <p>Skip the install and configuration process with pre-build open source images supporting Rails, Cassandra, Docker, and more.</p>
                        </div>

                        <div class="col-12 col-md-6">
                            <img src="../../assets/img/global.svg" alt="Global availability">
                            <h4 class="fw-bold mt-2">Global availability</h4>
                            <p>Deploy to any of our data center regions around the world.</p>
                        </div>
                        
                    </div>
                </div>

            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'Deploy'
}
</script>

<style lang='scss' scoped>

p, li {
    color: #606e8c;
}

</style>