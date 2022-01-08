<template>
    <section>
        <div class="container py-5">

            <h2 class="text-center fw-bold mb-4">Get started now.</h2>
            
            <div class="text-center">
                <button class="border-0 rounded px-3 py-2">Create your account</button>
            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'GetStartBottom'
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

section {
    @include mainColorGradient;

    h2 {
        color: #fff;
    }

    button {
        color: $mainColor;
        background-color: #fff;
        transition: all .3s;

        &:hover {
            color: #fff;
            background-color: $mainColor;
        }
    }
}

</style>