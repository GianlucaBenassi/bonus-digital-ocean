<template>
    <header class="position-relative">
        <div class="container h-100">

            <div class="row h-100">

                <!-- left -->
                <div class="col-10 col-lg-3 h-100">
                    <!-- logo -->
                    <a href="#" class="d-flex align-items-center h-100 logo">
                        <img src="../../assets/img/logo.png" alt="Digital Ocean top logo">
                    </a>
                </div>

                <!-- right -->
                <div class="col-2 col-lg-9 h-100">
                    <!-- navbar -->
                    <nav class="d-flex d-lg-block justify-content-end align-items-center h-100">

                        <!-- nav list -->
                        <div class="row d-lg-flex align-items-center nav_lists" :class="{ms_close : menuClose}">

                            <div class="col-12 col-lg-6 text-lg-center">
                                <ul class="m-lg-0 p-lg-0">
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <a href="#">Products<i class="fas fa-chevron-down"></i></a>
                                    </li>
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <a href="#">Customers</a>
                                    </li>
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <a href="#">Community<i class="fas fa-chevron-down"></i></a>
                                    </li>
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <a href="#">Pricing</a>
                                    </li>
                                </ul>
                            </div>

                            <div class="col-12 col-lg-6 text-lg-end">
                                <ul class="m-lg-0 p-lg-0">
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <a href="#">Docs</a>
                                    </li>
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <a href="#">Support<i class="fas fa-chevron-down"></i></a>
                                    </li>
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <a href="#">Login</a>
                                    </li>
                                    <li class="d-lg-inline-block my-2 my-lg-0 mx-lg-1 mx-xl-2">
                                        <button class="ms_login rounded px-2 py-1">Sing Up</button>
                                    </li>
                                </ul>
                            </div>
                            
                        </div>

                        <!-- nav open menu button -->
                        <div @click="openMenu()" :class="{ms_close : menuButtonHide}">
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

    .logo img {
        height: 70%;
    }

    nav {

        .nav_lists {
            position: absolute;
            top: 50px;
            left: 0;
            right: 0;
            z-index: 9999;
            
            li a {
                color: #000;
                transition: all .2s;

                .fa-chevron-down {
                    font-size: .8em;
                    margin-left: 2px;
                }

                &:hover {
                    color: $mainColor;
                }
            }

            .ms_login {
                color: $mainColor;
                background-color: #fff;
                border: 1px solid $mainColor;
                transition: all .3s;

                &:hover {
                    color: #fff;
                    background-color: $mainColor;
                }
            }

            @media screen and (min-width: 992px) {
                & {
                    position: inherit;
                    height: 100%;
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