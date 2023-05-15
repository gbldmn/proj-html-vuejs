<script>
export default {
    name: "SearchComp",
    props: {
        menu: Array
    }
    }
</script>

<template>
    <div class="d-flex justify-content-between h-150 align-items-center wt">
        <div>
            <img width="150" src="images/dark-logo.png" alt="">
        </div>
        <div class="align-items-center">
            <ul class="mt-2">
                <li v-for="(elemMenu, index) in menu" :key="index"  class="d-inline-block menu-item position-relative">
                     <a href="#">{{ elemMenu.nome }} <i class="fa-solid fa-chevron-down" style="color: #000000;"></i></a>
                     <ul class="sub-menu position-absolute " v-if="(elemMenu.subMenu.length)">
                        <li v-for="(elem, index) in elemMenu.subMenu" :key="index">
                           <a href="">{{ elem }}</a> 
                        </li>
                     </ul>
                </li>
                <li class="d-inline-block"> <a href="#"> <i class="fa-regular fa-circle-user d" style="color: #000000;"></i> </a> </li>
                <input  type="text" placeholder="Search..."> <button> <i class="fa-solid fa-magnifying-glass"></i> </button>
            </ul>
            
        </div>
    </div>
</template>


<style lang="scss" scoped>
.wt {
    width: 80%;  
    margin: 0 auto;
}
    input {
    padding: 0.5rem;
    font-weight: bold;
    font-size: 15px;
    border: 1px solid #20AD96;
    border-radius: 10px 0px 0px 10px;
    margin-top: 20px;
    border-right: 1px solid white;
}
button {
    padding: 0.5rem;
    font-weight: bold;
    font-size: 15px;
    border: 1px solid #20AD96;
    border-radius: 0px 10px 10px 0px;
    color: white;
    margin-top: 20px;
    border-left: 1px solid white;
    i {
        color: grey;
    }
}
button:hover {
    background-color: #20AD96;
    i {
        color: white;
    }
}
.sub-menu {
    display: none;
    z-index: 99999;
    background-color: white;
    padding: 1rem;
    border-bottom: 4px solid #20AD96;
}
.menu-item:hover .sub-menu {
    display: block;
}
ul li {
    list-style-type: none;
    line-height: 1.5rem;
}


</style>