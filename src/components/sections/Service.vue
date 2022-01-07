<template>
    <section>
        <div class="container py-5">

            <h2 class="text-center">Service your customers around the world from 12 regions.</h2>

            <div class="row row-cols-1 row-cols-lg-2">

                <div class="col">
                    <ul class="p-0">

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">ams2</h6>
                            <span class="flex-fill">Amsterdam, Netherlands</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">ams3</h6>
                            <span class="flex-fill">Amsterdam, Netherlands</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">blr1</h6>
                            <span class="flex-fill">Bangalore, India</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">fra1</h6>
                            <span class="flex-fill">Frankfurt, German</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">lon1</h6>
                            <span class="flex-fill">London, UK</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">nyc1</h6>
                            <span class="flex-fill">New York, USA</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                    </ul>
                </div>

                <div class="col">
                    <ul class="p-0">

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">ams2</h6>
                            <span class="flex-fill">Amsterdam, Netherlands</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">ams3</h6>
                            <span class="flex-fill">Amsterdam, Netherlands</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">blr1</h6>
                            <span class="flex-fill">Bangalore, India</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">fra1</h6>
                            <span class="flex-fill">Frankfurt, German</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex border-bottom border-light py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">lon1</h6>
                            <span class="flex-fill">London, UK</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                        <li class="d-flex py-2">
                            <h6 class="me-3 me-sm-5 mb-0 text-uppercase lh-base">nyc1</h6>
                            <span class="flex-fill">New York, USA</span>
                            <a href="#">Test speed &gt;</a>
                        </li>

                    </ul>
                </div>

            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'Service'
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

section {
    @include mainColorGradient;
    color: #fff;
}

a {
    color: #00bdcf;
    
    &:hover {
        color: #00bdcf;
        text-decoration: underline;
    }
}

</style>