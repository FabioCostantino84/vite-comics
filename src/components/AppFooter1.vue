<script>
export default {

    name: "AppFooter1",
    data() {
        return {

        }
    }
}

</script>


<template>

    <div class="f_container">

        <div class="container w-75 m-auto">

            <div class="row">
                <div class="d-flex col-6 mt-4">
                   
                        <div class="d-flex flex-column">
                            <h3>DC COMICS</h3>
                            <a href="">Characters</a>
                            <a href="">Comics</a>
                            <a href="">Movies</a>
                            <a href="">TV</a>
                            <a href="">Games</a>
                            <a href="">Videos</a>
                            <a href="">News</a>
    
                            <h3>SHOP</h3>
                            <a href="">Shop DC</a>
                            <a href="">Shop DC Collectibles</a>
                        </div>
                        <div class="d-flex flex-column ps-5">
                            <h3 class="">DC</h3>
                            <a href="">Terms Of Use</a>
                            <a href="">Privacy Policy (New)</a>
                            <a href="">Add Choices</a>
                            <a href="">Advertising</a>
                            <a href="">Jobs</a>
                            <a href="">Subscription</a>
                            <a href="">Talent Workshops</a>
                            <a href="">CPSC Certificates</a>
                            <a href="">Ratings</a>
                            <a href="">Shop Help</a>
                            <a href="">Contact Us</a>
                        </div>
                        <div class="d-flex flex-column ps-5">
                            <h3>SITES</h3>
                            <a href="">DC</a>
                            <a href="">MAD Magazine</a>
                            <a href="">DC Kids</a>
                            <a href="">DC Universe</a>
                            <a href="">DC Power Visa</a>
                        </div>
    
                </div>
    
                <div class="col-6">
                    <div class="box">
                        
                        <img src="../assets/img/dc-logo-bg.png" alt="">
    
                    </div>
                </div>
            </div>

        </div>

    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.f_container {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    /* height: 200px; */
}

.box {
    width: 500px;
    height: 360px;
    overflow: hidden;
}
.box > img {
    height: 500px;
    width: 500px;
    margin-top: -85px;
}

h3 {
    color: #ffffff;
}

a{
    text-decoration: none;
    color: gray;
}
</style>
