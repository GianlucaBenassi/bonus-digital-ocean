<template>
    <div class="position-absolute bottom-0 m-3">

    </div>
</template>

<script>
export default {
    name: 'Help'
}
</script>

<style lang='scss' scoped>

div {
    left: 0;
    z-index: 9998;


    background-color: red;
    height: 200px;
    width: 250px;

    @media screen and (min-width: 992px) {
        & {
            left: inherit;
            right: 0;
        }
    }
}

</style>