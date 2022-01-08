<template>
    <footer>
        <div class="container py-5">

            <div class="row">

                <!-- social column -->
                <div class="col-12">
                    <img src="../../assets/img/logo-small.svg" alt="DigitalOcean small logo">
                    <span class="d-block mt-2"><i class="far fa-copyright"></i> 2018 DigitalOcean, LLC. All rights reserved.</span>
                    <span class="d-block">Proudly made in NY</span>
                    <ul class="d-flex p-0">
                        <li class="me-2">
                            <a href="#" class="fs-5"><i class="fab fa-twitter"></i></a>
                        </li>
                        <li class="me-2">
                            <a href="#" class="fs-5"><i class="fab fa-facebook-square"></i></a>
                        </li>
                        <li class="me-2">
                            <a href="#" class="fs-5"><i class="fab fa-instagram"></i></a>
                        </li>
                        <li class="me-2">
                            <a href="#" class="fs-5"><i class="fab fa-youtube"></i></a>
                        </li>
                        <li class="me-2">
                            <a href="#" class="fs-5"><i class="fab fa-linkedin"></i></a>
                        </li>
                    </ul>
                </div>

                <!-- links column -->
                <div class="col-12">

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
    }
}

</style>