<script>

export default {
    name: "MainComp3.vue",
    data(){
        return {
            cards: [
                {
                    "titolo": "It's a choice of quality for people eith special  needs",
                    "testo": "I 'm a very person so i require everything to be organized and neat. Then, i'll be able to make things right and shine. MaxCoach guys just got me.",
                    "foto": "images/testimonial-avata-03.jpg",
                    "nome": "FLORENCE THEMES",
                    "lavoro": "/ multimedia admin"
                },
                {
                    "titolo": "High level of efficiency and scirntific teaching methods",
                    "testo": "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
                    "foto": "images/testimonial-avata-02.jpg",
                    "nome": "NINA HOLLACE",
                    "lavoro": "/ Freelancer"
                },
                {
                    "titolo": "Professional team of specialists and passionate mentors at reach",
                    "testo": "I need to get a certification for English proficiecy and MaxCoach is my best choice. Their tutors ar smart and professional when dealing with students.",
                    "foto": "images/testimonial-avata-04.jpg",
                    "nome": "MADLEY PONDOR  ",
                    "lavoro": "/ IT specialist"
                }
            ],
            arrayC: [
                {
                    "p": "Successfully trained",
                    "number": "1790",
                    "blog": "ENROLLED LEARNERS"
                },
                {
                    "p": "Proudly Received",
                    "number": "19",
                    "blog": "COUNTRYWIDE AWARDS"
                },
                {
                    "p": "Firmly Established",
                    "number": "24",
                    "blog": "LOCAL BRANCHES"
                },
                {
                    "p": "Getting Featured on",
                    "number": "1090",
                    "blog": "BLOG POSTS"
                }
            ],
        }
    }
}

</script>

<template>
<div class="box ">
  <div class="mt-5 p-4 ccc">
        <h6 class="color-3">CREATE WORDS ABOUT MAXCOACH</h6>
        <h4 class="color-2">Our <span class="color"> top learners'</span> verbatim </h4>
  </div>

    <div class="box2 d-flex p-5 justify-content-between">
     
        <div v-for="(elem, index) in cards" :key="index" class="card d-flex " style="width: 29rem;">
            <div class="card-body">
                <h5 class="card-title color-2">{{ elem.titolo }}</h5>
                <p class="card-tex color">{{ elem.testo }}</p>
                <div class="d-flex">
                    <div>
                        <img  width="40" class="rounded-circle me-2" :src="elem.foto" alt="">
                    </div>
                    <div>
                        <span>{{ elem.nome }}</span>
                        <h6>{{ elem.lavoro }}</h6>
                    </div>
                </div>
            </div>
        </div>
    </div>
 
    <div class="box3 d-flex justify-content-center align-items-center">
        <div>
            <img src="images/maxcoach-shape-01.png" alt="">
            <img class="m" width="40" src="images/maxcoach-shape-05-150x150.png" alt="">
        </div>
        <div class="text-center margin lh-lg">
            <h5 class="color-2">start today for getting <span class="color">online certification</span></h5>
            <h4 class="color-2">You can be your own guiding star whit our help!</h4>
            <button>Get started now</button>
        </div>
        <div>
            <img src="images/maxcoach-shape-02.png" alt="">
        </div>
    </div>
 <div class="box5">
    <div class="box4 d-flex  lh-lg">
        <div v-for="(elem, index) in arrayC" :key="index" class="items2 d-flex flex-column justify-content-center align-items-center  lh-lg">
            <p class="color-2">{{ elem.p }}</p>
            <h1 class="color"> <strong>{{ elem.number }}</strong> </h1>
            <p class="color-3">{{ elem.blog }}</p>
        </div>

    </div>
    </div>
  
</div>

</template>


<style lang="scss" scoped>
.box {
    width: 100%;
    background-color: #F8F8F8;
}
.color {
    color: #20AD96;
}
.color-2 {
    color: #3F3A64;
}
.color-3 {
    color: #A9A7BA;
}
.box2 {
    width: 100%;
    margin: 0 auto;
}
.items {
    width: calc(100% / 3 - 2px);
}
.ccc {
    margin-left: 650px;
}
.box3 {
    width: 80%;
    margin: 0 auto;
    height: 350px;
}
button {
    padding: 1rem;
    font-weight: bold;
    font-size: 15px;
    background-color: #20AD96;
    border: 1px solid #20AD96;
    border-radius: 10px;
    color: white;
    margin-top: 20px;
}
.margin {
    margin-left: 100px;
    margin-right: 100px;
}
.m {
    margin-bottom: 100px;
}
.items2 {
    width: calc(100% / 4);
    border-left: 1px solid #F4F0EC;
    border-right: 1px solid #F4F0EC;
}
.box4 {
    width: 80%;
    margin: 0 auto;
    height: 350px;
    background-color: white;
}
.box5 {
    width: 100%;
    background-color: white;
}

</style>