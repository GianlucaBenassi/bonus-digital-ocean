<template>
    <div class="position-absolute d-flex flex-column flex-lg-row-reverse align-items-lg-end bottom-0 m-3">

        <!-- shark image -->
        <div class="position-relative d-flex align-items-center rounded ms-lg-3 ms_image">
            <img src="../../assets/img/shark.png" alt="Help shark" class="w-100">
            <span class="position-absolute d-flex justify-content-center align-items-center text-center border border-3 border-light rounded-circle">2</span>
        </div>

        <!-- text card -->
        <div class="position-relative rounded mt-3 mt-lg-0 p-2 ms_card">
            <p class="m-0">Can i help answer any questions you have about DigitalOcean?</p>
            <div class="ms_tip position-absolute"></div>
        </div>

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

    .ms_image {
        width: 60px;
        height: 60px;
        background-color: #006aff;

        span {
            width: 27px;
            height: 27px;
            font-size: .8rem;
            color: white;
            background-color: #ff0001;
            bottom: 40px;
            left: 40px;
        }
    }

    .ms_card {
        background-color: #fff;
        width: 270px;

        .ms_tip {
            width: 20px;
            height: 20px;
            background-color: #fff;
            left: 253px;
            top: 36px;
            transform: rotate(45deg);
        }
    }

    @media screen and (min-width: 576px) {
        .ms_card {
            width: 335px;

            .ms_tip {
                left: 318px;
            }
        }
    }

    @media screen and (min-width: 992px) {
        & {
            left: inherit;
            right: 0;
        }
    }
}

</style>