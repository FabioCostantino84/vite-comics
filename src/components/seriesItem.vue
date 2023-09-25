<script>

export default {
    name: 'seriesItem',
    props: ['image', 'title', 'cardsArray', 'cards', 'card']


}

</script>



<template>
    
    <div class="card flex-nowrap bg-transparent py-3">
        <img :src="image" class="imgSeries" alt="title">
        <div class="card-body">
            <h4 class="card-text text-white text-start">{{ title }}</h4>
        </div>
    </div>
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.imgContainer {
    background-image: url(../assets/img/jumbotron.jpg);
    height: 450px;
    background-size: cover;

}

.card {
    border: none;
}

.imgSeries {
    height: 200px;
}






</style>