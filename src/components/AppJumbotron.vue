<script>
export default {

    name: "AppJumbotron",

    data() {
        return {
        }
    }
}

</script>


<template>
    <div class="jumbotron">

        <div class="container w-75 m-auto align-items-md-stretch">

            <div class="py-5 text-white">
                <h2>Content goes here</h2>
            </div>
        </div>

    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.jumbotron {
    background-color: $black-color;
}
</style>