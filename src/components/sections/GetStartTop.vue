<template>
    <section>
        <div class="container">
            <div class="row py-5">
                
                <!-- title column -->
                <div class="col-12 col-md-7 ms_description">
                    <h1 class="fw-bold">The simplest cloud platform for developers & teams</h1>
                    <p>Deploy, manage, and scale cloud applications faster and more efficiently on DigitalOcean. We make managing infrastructure easy for teams and businesses, wheather you're running one virtual machine or ten thousand.</p>
                </div>

                <!-- google login form -->
                <div class="col-12 col-md-5">
                    <form class="rounded pt-4 pb-2 px-2" @submit.prevent>

                        <h4 class="fw-bold text-center">Deploy your app in seconds.</h4>
                        <h4 class="fw-bold text-center ms_color">Get started now.</h4>

                        <input class="w-100 mb-2 px-1" type="email" placeholder="Email">
                        <input class="w-100 mb-2 px-1" type="password" placeholder="Password">

                        <button class="d-block rounded w-100 mb-2 ms_create">Create your account</button>
                        <button class="d-block position-relative border rounded w-100 mb-2 ms_google">
                            <img class="position-absolute top-50 translate-middle" src="../../assets/img/google-icon.png" alt="google logo">
                            Sing up with google
                        </button>

                        <p class="text-center">By signign up you agree to the <a href="#">Terms of Service</a>.</p>
                    </form>
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

@import '../../assets/style/variables.scss';

section {
    background-image: url('../../assets/img/bg-banner-home.jpg');
    background-position: center;
    background-size: cover;

    .ms_description {
        color: #fff;
    }

    form {
        background-color: #fff;

        .ms_color {
            color: $mainColor;
        }

        .ms_create {
            color: #fff;
            background-color: #579aff;
            border: 1px solid #579aff;
            transition: all .3s;

            &:hover {
                color: $mainColor;
                background-color: #fff;
            }
        }

        .ms_google {
            background-color: #fff;
            transition: all .3s;
            
            img {
                max-height: 16px;
                left: 14px;

            }

            &:hover {
                background-color: #efefef;
            }
        }

        p {
            font-size: 12px;

            a:hover {
                text-decoration: underline;
            }
        }
    }
}

</style>