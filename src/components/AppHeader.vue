<script>
export default {

    name: "AppHeader",

    data() {
        return {

            navLink: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop'],
        }
    }
}

</script>


<template>
    <header>

        <div class="container w-75">
            <div class="row align-items-center">
                <div class="col-4">

                    <!-- LOGO -->
                    <img src="../assets/img/dc-logo.png" alt="">

                </div>
                <div class="col-8 d-flex justify-content-center">

                    <!-- NAVBAR -->
                    <nav class="navbar navbar-expand-sm ">

                        <!-- CICLO NELL' ARRAY -->
                        <div v-for="link in navLink" class="container-fluid">
                            <a class="nav-link active text-uppercase font-weight-bold align-content-center"
                                aria-current="page" href="#">{{ link }}</a>

                            <!-- <a class="navbar-brand" href="#">COMICS</a>
                            <a class="navbar-brand" href="#">MOVIES</a>
                            <a class="navbar-brand" href="#">TV</a>
                            <a class="navbar-brand" href="#">GAMES</a>
                            <a class="navbar-brand" href="#">COLLECTIBLES</a>
                            <a class="navbar-brand" href="#">VIDEOS</a>
                            <a class="navbar-brand" href="#">FANS</a>
                            <a class="navbar-brand" href="#">NEWS</a>
                            <a class="navbar-brand" href="#">SHOP</a> -->

                        </div>
                    </nav>

                </div>
            </div>
        </div>

    </header>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.col-8 {
    font-weight: bolder;
}

a:hover{
    border-bottom: 3px solid $primary-color;
    color: $primary-color;

}
</style>