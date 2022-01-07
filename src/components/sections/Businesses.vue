<template>
    <section>
        <div class="container text-center py-5">

            <h6 class="text-uppercase">Innovative businesses trust digitalocean</h6>

            <div class="row row-cols-2 row-cols-md-6">
                
                <div class="col d-flex align-items-center">
                    <img class="w-100" src="../../assets/img/docker.svg" alt="docker logo">
                </div>
                
                <div class="col d-flex align-items-center">
                    <img class="w-100" src="../../assets/img/gitlab.svg" alt="gitlab logo">
                </div>
                
                <div class="col d-flex align-items-center">
                    <img class="w-100" src="../../assets/img/slack.svg" alt="slack logo">
                </div>
                
                <div class="col d-flex align-items-center">
                    <img class="w-100" src="../../assets/img/hashicorp.svg" alt="hashicorp logo">
                </div>
                
                <div class="col d-flex align-items-center">
                    <img class="w-100" src="../../assets/img/hashicorp.svg" alt="hashicorp_2 logo">
                </div>
                
                <div class="col d-flex align-items-center">
                    <img class="w-100" src="../../assets/img/splunk.svg" alt="splunk logo">
                </div>

            </div>

            <a href="#" class="d-block">View customer stories ></a>

        </div>
    </section>
</template>

<script>
export default {
    name: 'Businesses'
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

section {
    background-color: $sectionColor;

    a {
        color: $mainColor;

        &:hover {
            text-decoration: underline;
        }
    }
}

</style>