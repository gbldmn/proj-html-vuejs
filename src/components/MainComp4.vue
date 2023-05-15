<script>
export default {
    name: "MainComp4.vue",
    }
</script>

<template>
<div class="box">
    <div class="box2 d-flex justify-content-between align-items-center">
        <div class="d-flex flex-column">
            <h6 class="color-2"> ENJOYABLE INSIGHTS</h6>
            <h3 class="color-2"> Most Viewed <span class="color">Best Blogs</span></h3>
  
                <p class="lh-lg mt-4 color-2"> <i class="fa-solid fa-arrow-right-long"></i> <strong> Become a Better Blogger:Content Planning</strong></p>
                <p class="lh-lg color-2"> <i class="fa-solid fa-arrow-right-long"></i> <strong> Promoting Your Online Business on Pinterest</strong></p>
                <p class="lh-lg color-2"> <i class="fa-solid fa-arrow-right-long"></i> <strong> Gamification and Game-Based Learning</strong></p>
                <p class="lh-lg color-2"> <i class="fa-solid fa-arrow-right-long"></i> <strong> Designing on Course from Expert's Perspectiv</strong>e</p>
                <p class="lh-lg color-2"> <i class="fa-solid fa-arrow-right-long"></i> <strong> Why Online Courses Are the Future of Education</strong></p>
 
        </div>
        <div>
            <div class="card" style="width: 25rem;">
                <div class="good">
                    <img src="images/artist-blog-03-480x352.jpeg" class="card-img-top" alt="...">
                </div>
                <div class="card-body">
                    <h5 class="card-title color-3">ARTIST</h5>
                    <p class="card-text color-2"> <strong> Brush Strokes Energize trees in Paintings</strong></p>
                    <p class="color-3"> <i class="fa-regular fa-calendar"></i> May 15, 2020  <i class="fa-regular fa-eye"></i> 688 views </p>
                </div>
            </div>
        </div>
        
        <div> 
            <div class="card" style="width: 23.5rem;">
                <div class="good">
                   <img src="images/artist-blog-01-480x352.jpg" class="card-img-top" alt="...">
                </div>
                 <div class="card-body">
                    <h5 class="card-title color-3">ARTIST</h5>
                    <p class="card-text color-2"> <strong> Pocket-Sized Notebooks Hold Miniature Paintings</strong></p>
                    <p class="color-3"> <i class="fa-regular fa-calendar"></i> May 15, 2020  <i class="fa-regular fa-eye"></i> 603 views </p>
                 </div>
            </div>
        </div>
    </div>
</div>

</template>






<style lang="scss" scoped>
.good {
    overflow: hidden;
    width: 100%;
    height: 100%px;
}
img {
    transition: all 0.7s ease-in-out;
}
.good:hover img {
    transform: scale(1.7);
    filter: brightness(0.7);
}

.box {
    width: 100%;
    background-color: #F4F0EC;
    height: 650px;
}
.box2 {
    width: 80%;
    margin: 0 auto;
    height: 100%;
}
ul li {
    list-style-type: none;
}
.color-2 {
    color: #3F3A64;
}
.color-3 {
    color: #A9A7BA;
}
.color {
    color: #20AD96;
}
p:hover {
    color: #20AD96;
    cursor: pointer;
}
</style>