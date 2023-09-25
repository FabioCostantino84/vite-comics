<script>
import cards from '../card.js'
export default {

    name: "AppJumbotron",

    data() {
        return {
            cards,
        }
    }
}

</script>


<template>
    <div class="jumbotron">

        <div class="imgContainer"></div>

        <div class="container text-center py-5">
            <div class="row row-cols-6">
                <div v-for="card in cards.cards" class="card flex-nowrap bg-black py-3">
                    <img :src="card.thumb" class="imgSeries" alt="...">
                    <div class="card-body">
                        <h4 class="card-text text-white text-start">{{ card.series }}</h4>
                    </div>
                </div>
            </div>
        </div>

        <!-- <div class="container w-75 m-auto align-items-md-stretch">

            <div class="py-5 text-white">
                <h2>Content goes here</h2>
            </div>
        </div> -->

    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.jumbotron {
    background-color: $black-color;
}

.imgContainer {
    background-image: url(../assets/img/jumbotron.jpg);
   height: 450px;
   background-size: cover;

}

.imgSeries {
    height: 200px;
}
</style>