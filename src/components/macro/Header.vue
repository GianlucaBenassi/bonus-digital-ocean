<template>
    <header>
        <div class="container">

            <div class="row main_row">

                <!-- left -->
                <div class="col-10 col-lg-4">
                    <!-- logo -->
                    <a href="#" class="logo">
                        <img src="../../assets/img/logo.png" alt="Digital Ocean top logo">
                    </a>
                </div>

                <!-- right -->
                <div class="col-2 col-lg-8">
                    <!-- navbar -->
                    <nav>

                        <!-- nav list -->
                        <div class="row nav_lists" :class="{close : menuClose}">
                            <div class="col-12">
                                bla bla
                            </div>
                            <div class="col-12">
                                bla bla
                            </div>
                        </div>

                        <!-- nav open menu button -->
                        <div @click="openMenu()" :class="{close : menuButtonHide}">
                            <i class="fas fa-bars"></i>
                        </div>

                    </nav>
                </div>

            </div>

        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            menuClose: false,
            menuButtonHide: true
        }
    },
    methods: {
        OnResize() {
            if (window.innerWidth < 992) {
                this.menuClose = true;
                this.menuButtonHide = false;
            } else {
                this.menuClose = false;
                this.menuButtonHide = true;
            }
        },
        openMenu() {
            this.menuClose = !this.menuClose;
        }
    },
    mounted() {
        this.OnResize();
        window.addEventListener('resize', this.OnResize, {passive: true});
    }
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

header {
    height: 50px;
    position: relative;
    background-color: green;

    .container {
        height: 100%;

        .main_row {
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

        .nav_lists {
            position: absolute;
            top: 50px;
            left: 0;
            right: 0;

            background-color: red;

            @media screen and (min-width: 992px) {
                & {
                    position: relative;
                    top: 0;
                }
            }
        }

        .fa-bars {
            color: $mainColor;
            cursor: pointer;
        }
    }
}

</style>