<script>
export default {
    name: "MainComp2.vue",
    data(){
        return {
            cards: [
                {
                    "thumb": "images/artist-blog-01-480x352.jpg",
                    "price": "$40,00",
                    "lavoro": "Learning to write as a Professional Author",
                    "lessons": "20",
                    "students": "50"
                },
                {
                    "thumb": "images/stock-full-hd-03-480x298.jpg",
                    "price": "Free",
                    "lavoro": "Customer-centric Info-Tech Strat",
                    "lessons": "24",
                    "students": "769"
                },
                {
                    "thumb": "images/stock-full-hd-04-480x298.jpg",
                    "price": "$19,00",
                    "lavoro": "Open programming courses for everyone",
                    "lessons": "17",
                    "students": "62"
                },
                {
                    "thumb": "images/stock-full-hd-05-480x298.jpg",
                    "price": "$26,00",
                    "lavoro": "Academic listening and note-taking",
                    "lessons": "14",
                    "students": "67"
                },
                {
                    "thumb": "images/stock-full-hd-06-480x298.jpg",
                    "price": "$39,00",
                    "lavoro": "Master jquery in a short period of time",
                    "lessons": "6",
                    "students": "51"
                },
                {
                    "thumb": "images/artist-blog-01-480x352.jpg",
                    "price": "$59,00",
                    "lavoro": "Introduction to javascript for beggines",
                    "lessons": "14",
                    "students": "76"
                },
            ]
        }
    }
}


</script>

<template>
<div class="box text-center">
    <div class="box2 d-flex flex-column">
        <div class="box3  d-flex flex-column justify-content-center aligh-items-end">
           <div class="text-center">
            <span>Stimulated to learn</span>
            <h2>Featured Online Courses</h2>
           </div>
        </div>
        <div class="box4 d-flex flex-row ">
            <div v-for="(elem,index) in cards" :key="index" class="cards d-flex flex-row mb-4 mt-2 ">
                <img class=" img me-2" :src="elem.thumb" alt="">
                <div class="d-flex align-items-start flex-column">
                    <h4 class="mt-4"> {{ elem.price }} </h4>
                    <h5> {{ elem.lavoro }} </h5>
                    <p class="d-inline-block"> <i class="fa-regular fa-file-lines"></i> {{ elem.lessons }} lessons <i class="fa-regular fa-user"></i> {{ elem.students }} students</p>
                    <!-- <span> <i class="fa-regular fa-user"></i> {{ elem.students }} </span> -->
                </div>
            </div>
        </div>
    </div>
    <button class="text-center mt-3 mb-4">view all courses <i class="fa-solid fa-arrow-right" style="color: #ffffff;"></i> </button>
</div>

<div class="box4">
    <div class="box2 text-center mt-5">
        <span>Maxcoach available courses</span>
        <h2>Access smart tutoring program for benefits.</h2>
    </div>
    <div class="box2 d-flex justify-content-between flex-wrap">
        <div class="mt-4">
            <div class="card" style="width: 18rem;">
                 <img src="images/home-2-image-box-01.png" class="card-img-top" alt="...">
                 <div class="card-body">
                 <h5 class="card-title">Customize preferences</h5>
                 <p class="card-text">Learners are given the right to arrange and customize there study schedule and timetable based on preferences.</p>
                 <a href="#">Start Here <i class="fa-solid fa-arrow-right"></i> </a>
                </div>
            </div>
        </div>
        <div class="mt-4">
            <div class="card" style="width: 18rem;">
                 <img src="images/about-us-02-image-box-02.png" class="card-img-top" alt="...">
                 <div class="card-body">
                  <h5 class="card-title">Cloud storage</h5>
                  <p class="card-text">You can store online lessons via online cloud or dowload to your device and revice lessons on the way.</p>
                  <a href="#">Get Free Quote <i class="fa-solid fa-arrow-right"></i> </a>
                 </div>
            </div>
        </div>
        <div class="mt-4">
            <div class="card" style="width: 18rem;">
                <img src="images/home-2-image-box-03.png" class="card-img-top" alt="...">
                  <div class="card-body">
                  <h5 class="card-title">Multimedia channels</h5>
                  <p class="card-text">We provide study materials whit barious formats: video, audio, slaits, doc, prints, books and applications.</p>
                  <a href="#">Start Now <i class="fa-solid fa-arrow-right"></i> </a>
                  </div>
            </div>
        </div>
    </div>
  <div class="den d-flex mt-5 position-relative">
    <img class="position-absolute zi mt-4 ms-5" width="500" src="images/home-2-popup-video-poster.jpg">
    <div class=" dert d-flex align-items-end flex-column position-relative"> 
        <!-- <img class="mt-2 me-auto position-absolute zii" width="100" src="images/icon-youtube-play.png"> -->
         <img class="mt-2 me-auto"  src="images/maxcoach-shape-05-100x100.png">
         <img class="mt-2 mt-auto"  src="images/maxcoach-shape-08.png">
     </div>
     <div class="d-flex justify-content-center align-items-center dert">
        <div>
            <h6 class="coler">GET STARTED <span class="color">AFFORTLESSY</span> </h6>
            <h1>Enjoy our <br> <span class="color-2">componiorship</span></h1>
            <p>Sneek peek into what as in store for you on our <br> online teaching and mantoring portal. Seek for <br>
            some hidden hints of early-bird rewards as well.</p>
            <a class="color-2" href="#">dowload free guidebook <i class="fa-solid fa-arrow-right"></i> </a>
        </div>
     </div>
    </div>
</div>

</template>

<style lang="scss" scoped>
.box {
    width: 100%;
    background-color: #F5F7FA;
}
.box2 {
    margin: 0 auto;
    width: 80%;

}
.box3 {
    width: 100%;
    height: 200px;
}
.box4 {
    width: 100%;
}
.cards {
    width: calc(100% / 2 - 1px);
    background-color: #F5F7FA;
}
.img {
    width: 150px;
    border-radius: 100%;
}
.flex-row {
    flex-wrap: wrap;
}
h4 {
    color: #20AD96;
}
p {
    color: #20AD96;
}
.mt-3 {
    padding: 1rem;
    font-weight: bold;
    font-size: 15px;
    background-color: #20AD96;
    border: 1px solid #20AD96;
    border-radius: 10px;
    color: white;
}
a {
    text-decoration: none;
    color: #A9A7BA
}
h5 {
    color: #3F3A64;
}
.den {
    width: 80%;
    margin: 0 auto;
    height: 400px;
}
.dert {
    width: calc(100% / 2 );
}
.zii {
    z-index: 3;
    margin-top: 3rem;
}
.zi {
    z-index: 2;
    border-radius: 10px;
}
.color {
    color: #3F3A64;
}
.color-2 {
    color: #20AD96;
}
.coler {
    color: #A9A7BA;
}

</style>