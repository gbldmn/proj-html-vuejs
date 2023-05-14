<script>

export default {
    name: "PrefooterComp.vue",
}

</script>


<template>
    <div class="box">
        <div class="box3 d-flex justify-content-center align-items-center">
                <div>
                    <img src="images/maxcoach-shape-01.png" alt="">
                    <img class="m" width="40" src="images/maxcoach-shape-05-150x150.png" alt="">
                </div>
                <div class="text-center margin lh-lg">
                    <h4 class="color-2">Subscribe <span class="color">Newsletters</span></h4>
                    <p class="color-2">Enter your email address to register to our newsletter subscription <br> delivered on a regular basis!</p>
                    <input type="text" placeholder="Enter your email">
                    <button>subscribe</button>
                </div>
                <div class="item position-relative">
                    <img class="position-absolute g" src="images/maxcoach-shape-02.png" alt="">
                    <img class=" position-absolute c" src="images/maxcoach-shape-09.png" alt="">
                </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
.box {
    width: 100%;
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
    border-radius: 0px 10px 10px 0px;
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
input {
    padding: 1rem;
    font-weight: bold;
    font-size: 15px;
    border: 1px solid #20AD96;
    border-radius: 10px 0px 0px 10px;
    margin-top: 20px;
}
.item {
    width: 200px;
    height: 100%;
}
.g {
    margin-top: 100%;
    margin-left: 30%;
}
.c {
    margin-top: 30%;
}

</style>