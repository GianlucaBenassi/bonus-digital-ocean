<template>
    <section>
        <div class="container">
            <div class="row">
                
                <!-- title column -->
                <div class="col-12 ms_description">
                    <h1 class="mt-5 fw-bold">The simplest cloud platform for developers & teams</h1>
                    <p>Deploy, manage, and scale cloud applications faster and more efficiently on DigitalOcean. We make managing infrastructure easy for teams and businesses, wheather you're running one virtual machine or ten thousand.</p>
                </div>

                <!-- google login form -->
                <div class="col-12">

                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'GetStartTop.vue'
}
</script>

<style lang='scss' scoped>

section {
    background-image: url('../../assets/img/bg-banner-home.jpg');
    background-position: center;
    background-size: cover;

    height: 600px;

    .ms_description {
        color: #fff;
    }
}

</style>