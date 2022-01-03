<template>
    <header>
        <div class="container">

            <div class="row">

                <div class="col-10 col-lg-4">
                    <a href="#" class="logo">
                        <img src="../../assets/img/logo.png" alt="Digital Ocean top logo">
                    </a>
                </div>

                <div class="col-2 col-lg-8">
                    <nav>
                        <i class="fas fa-bars"></i>
                    </nav>
                </div>

            </div>

        </div>
    </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

header {
    height: 50px;

    .container {
        height: 100%;

        .row {
            height: 100%;

            & > * {
                height: 100%;
            }
        }
    }

    .logo {
        height: 100%;
        display: flex;
        align-items: center;

        img {
            height: 80%;
        }
    }

    nav {
        height: 100%;
        display: flex;
        justify-content: flex-end;
        align-items: center;

        .fa-bars {
            color: $mainColor;
            cursor: pointer;
        }
    }
}

</style>