<script>
export default {
    name: "MainComp.vue",
    }
</script>

<!-- PRIMA PARTE FINO AI SEI ADESIVI IN ORIZZONTALE -->

<template>
    <div class="text-end mt-4 d-inline-block ">
       <div><i class="fa-solid fa-cart-shopping mt-1"></i></div>
       <div><i class="fa-solid fa-book mt-1"></i></div>
       <div><i class="fa-regular fa-circle-stop mt-1"></i></div>
       <div><i class="fa-brands fa-codepen mt-1"></i></div>     
    </div>
    <div class="box margine">
        <div class="box2 d-flex">
            <div class="d-flex flex-column box3 justify-content-center  aligh-items-center">
                <div class="">
                    <h1> Distant learning for <br> further expansion</h1>
                    <p class="p">Learning is a life-long journey that in fact we never find <br> the terminate stop. Stop searching, enjoy the process</p>
                    <button class="mt-3"> <a class="cv" href=""> <i class="fa-solid fa-download" style="color: #ffffff;"></i> <strong> dowload free guide</strong> </a></button>
                    <p class="mt-3"> have a questions? <a href="#">Get free sample <i  class="fa-solid fa-arrow-right"></i> </a> </p>
                </div>
            </div>
            <div class="box3 d-flex flex-column justify-content-center  aligh-items-center position-relative">
                <img class="mb-2 tre " width="80" src="images/maxcoach-shape-07.png" alt="">
                <img class=" tre quattro " width="80" src="images/maxcoach-shape-07.png" alt="">
                <img class="rounded-circle position-absolute ms-4" width="430" src="images/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="">
                <img class="img tre" width="80" src="images/maxcoach-shape-07.png" alt="">
                <img class="position-absolute img2 tre quattro" width="80" src="images/maxcoach-shape-02.png" alt="">
            </div>
        </div>
        <div class="box4 d-flex justify-content-between h-300">
            <div><img width="60" src="images/client-logo-01.png" alt=""></div>
            <div><img width="60" src="images/client-logo-02.png" alt=""></div>
            <div><img width="60" src="images/client-logo-03.png" alt=""></div>  
            <div><img width="60" src="images/client-logo-04.png" alt=""></div>
            <div><img width="60" src="images/client-logo-05.png" alt=""></div>
            <div><img width="60" src="images/client-logo-06.png" alt=""></div>
        </div>
    </div>
</template>




<style lang="scss" scoped>
.box {
    width: 100%;
    height: 600px;
    background-color: white;
}
.box2 {
    width: 80%;
    margin: 0 auto;
    height: 80%;
}
.box3 {
    width: 50%;
    height: 100%;
}
.p {
    color: #A192A2;
}
h1 {
    color: #3F3A64;
}
button {
    background-color: #20AD96;
    color: white;
    border: 1px solid #20AD96;
    border-radius: 4px;
    padding: 15px;
    font-size: 10px;
}
a {
    font-weight: bold;
    color: #20AD96;
}
i {
    font-size: 15px;
}
.img {
    margin-top: 8rem;
    margin-left: 23rem;
}
.img2 {
    margin-left: 29rem;
    margin-bottom: 10rem;
}
.box4 {
    width: 80%;
    margin: 0 auto;
    height: 120px;
    margin-top: 10px;
}
.tre {
    transition: 2s;
}
.tre:hover {
    filter: grayscale(.6) sepia(.5);
    border-radius: 20px;
    transform: scale(1.5);
}
.quattro {
    animation: spin 2s linear infinite;
}
@keyframes spin {
    0% {
        transform: rotate(1turn);
    }
}
.cv {
    color: white;
}
.text-end {
    padding: 0.5rem;
    border: 1px solid grey;
    border-radius: 10px;
    position: fixed;
    z-index: 9999;
    display: flex;
    flex-direction: column;
    margin-left: 97%;
    background-color: white;
    i {
        color: #3F3A64;
        cursor: pointer;
    }
}
.margine {
    margin-top: 6rem;
}

</style>