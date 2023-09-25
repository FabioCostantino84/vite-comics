<script>
export default {

    name: "AppMainMenu",

    data() {
        return {

            menuCards: [
                {
                    text: 'digital comics',
                    image: './src/assets/img/buy-comics-digital-comics.png',
                },
                {
                    text: 'dc merchandise',
                    image: './src/assets/img/buy-comics-merchandise.png',
                },
                {
                    text: 'subscription',
                    image: './src/assets/img/buy-comics-subscriptions.png',
                },
                {
                    text: 'comic shop locator',
                    image: './src/assets/img/buy-comics-shop-locator.png',
                },
                {
                    text: 'dc power visa',
                    image: './src/assets/img/buy-dc-power-visa.svg',
                },
            ]
        }
    }
}

</script>


<template>
    <div class="mainMenu d-flex">

        <div class="row container m-auto my-5">
            <div class="d-flex flex-nowrap align-items-center align-content-between">
                <div v-for="card in menuCards" class="d-flex align-items-center">

                    <img :src="card.image" class="d-flex p-2">

                    <div class="text-white text-uppercase" style="">{{ card.text }}</div>
                </div>

            </div>
        </div>

    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.mainMenu {
    background-color: $primary-color;
}

img{
    width: 25%;
}
</style>
