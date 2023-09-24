<script>
export default {

    name: "AppFooter2",
    data() {
        return {

            brands: [
                {
                    name: 'facebook',
                    logo: 'src/assets/img/footer-facebook.png'
                },
                {
                    name: 'twitter',
                    logo: 'src/assets/img/footer-twitter.png'
                },
                {
                    name: 'youtube',
                    logo: 'src/assets/img/footer-youtube.png'
                },
                {
                    name: 'pinterest',
                    logo: 'src/assets/img/footer-pinterest.png'
                },
                {
                    name: 'periscope',
                    logo: 'src/assets/img/footer-periscope.png'
                },
            ]
        }
    }
}

</script>


<template>
    <footer>
        <div class="container w-75">
            <div class="row">
                <div class="col-12 d-flex align-items-center justify-content-between">
                    <div class="f_btn">
                        <a href="#" class="text-white text-uppercase text-decoration-none" role="button"
                            data-bs-toggle="button">sing-up now!</a>
                    </div>

                    <div class="d-flex align-items-center p-5">
                        <div>
                            <h4>FOLLOW US</h4>
                        </div>
                        <div v-for="brand in brands" class="iconsBrands d-flex flex-wrap p-2 align-items-center">
                            <img :src="brand.logo" :alt="brand.name">


                        </div>

                    </div>


                </div>

            </div>
        </div>
    </footer>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

footer {
    background-color: #303030;
}

h4 {
    color: $primary-color;
    padding: 1rem;
}

.f_btn {
    padding: 1rem;
    border: 0.25rem solid $primary-color;
}
</style>
