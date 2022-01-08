<template>
    <footer>
        <div class="container py-5">

            <div class="row">

                <!-- social column -->
                <div class="col-12 col-lg-5">
                    <img src="../../assets/img/logo-small.svg" alt="DigitalOcean small logo">
                    <span class="d-block mt-2"><i class="far fa-copyright"></i> 2018 DigitalOcean, LLC. All rights reserved.</span>
                    <span class="d-block">Proudly made in NY</span>
                    <ul class="d-flex p-0">
                        <li class="me-3">
                            <a href="#" class="fs-5"><i class="fab fa-twitter"></i></a>
                        </li>
                        <li class="me-3">
                            <a href="#" class="fs-5"><i class="fab fa-facebook-square"></i></a>
                        </li>
                        <li class="me-3">
                            <a href="#" class="fs-5"><i class="fab fa-instagram"></i></a>
                        </li>
                        <li class="me-3">
                            <a href="#" class="fs-5"><i class="fab fa-youtube"></i></a>
                        </li>
                        <li class="me-3">
                            <a href="#" class="fs-5"><i class="fab fa-linkedin"></i></a>
                        </li>
                    </ul>
                </div>

                <!-- links column -->
                <div class="col-12 col-lg-7">
                    <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4">

                        <div class="col">
                            <h6 class="fw-bold">Company</h6>
                            <ul class="p-0">
                                <li><a href="#">About</a></li>
                                <li><a href="#">Leadership</a></li>
                                <li><a href="#">Link</a></li>
                                <li><a href="#">Blog</a></li>
                                <li><a href="#">Carrers</a></li>
                                <li><a href="#">Partner Network</a></li>
                                <li><a href="#">Referreal Program</a></li>
                                <li><a href="#">Events</a></li>
                                <li><a href="#">Press</a></li>
                                <li><a href="#">Legal & Security</a></li>
                            </ul>
                        </div>

                        <div class="col">
                            <h6 class="fw-bold">Products</h6>
                            <ul class="p-0">
                                <li><a href="#">Droplets</a></li>
                                <li><a href="#">Spaces</a></li>
                                <li><a href="#">Kubernetes</a></li>
                                <li><a href="#">Load Balancers</a></li>
                                <li><a href="#">Block Storage</a></li>
                                <li><a href="#">Tools & Integrations</a></li>
                                <li><a href="#">One-Click Apps</a></li>
                                <li><a href="#">API</a></li>
                                <li><a href="#">Pricing</a></li>
                                <li><a href="#">Documentation</a></li>
                                <li><a href="#">Release Notes</a></li>
                            </ul>
                        </div>

                        <div class="col">
                            <h6 class="fw-bold">Community</h6>
                            <ul class="p-0">
                                <li><a href="#">Tutorials</a></li>
                                <li><a href="#">Meetups</a></li>
                                <li><a href="#">Q&A</a></li>
                                <li><a href="#">Write for Donations</a></li>
                                <li><a href="#">Droplets for Demos</a></li>
                                <li><a href="#">Hatch</a></li>
                                <li><a href="#">Shop Swag</a></li>
                                <li><a href="#">Research Program</a></li>
                                <li><a href="#">Currents Research</a></li>
                                <li><a href="#">Open Source</a></li>
                            </ul>
                        </div>

                        <div class="col">
                            <h6 class="fw-bold">Support</h6>
                            <ul class="p-0">
                                <li><a href="#">Contact Support</a></li>
                                <li><a href="#">FAQ</a></li>
                                <li><a href="#">Network Status</a></li>
                            </ul>
                        </div>

                    </div>
                </div>

            </div>

        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

footer {
    color: $textColor;
    background-color: #031c4e;

    ul li a {
        color: $textColor;

        &:hover {
            color: #fff;
        }
    }

    h6 {
        color: #fff;
    }
}

</style>