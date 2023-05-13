<script>
export default {
    name: "SearchComp",
    }
</script>

<template>
    <div class="d-flex justify-content-between h-150 align-items-center wt">
        <div>
            <img width="150" src="images/dark-logo.png" alt="">
        </div>
        <div class="align-items-center">
            <ul class="mt-2">
                <li class="d-inline-block"> <a href="#">Home <i class="fa-solid fa-chevron-down" style="color: #000000;"></i></a>  </li>
                <li class="d-inline-block"> <a href="#">Pages <i class="fa-solid fa-chevron-down" style="color: #000000;"></i></a>  </li>
                <li class="d-inline-block"> <a href="#">Courses <i class="fa-solid fa-chevron-down " style="color: #000000;"></i></a>  </li>
                <li class="d-inline-block"> <a href="#">Features <i class="fa-solid fa-chevron-down" style="color: #000000;"></i></a>  </li>
                <li class="d-inline-block"> <a href="#">Blog <i class="fa-solid fa-chevron-down" style="color: #000000;"></i></a>  </li>
                <li class="d-inline-block"> <a href="#">Shop <i class="fa-solid fa-chevron-down" style="color: #000000;"></i></a>  </li>
                <li class="d-inline-block"> <a href="#"> <i class="fa-regular fa-circle-user d" style="color: #000000;"></i> </a> </li>
                <input  type="text" placeholder="Search..."> <button> <i class="fa-solid fa-magnifying-glass"></i> </button>
                <button>gggg</button>
            </ul>
            
        </div>
    </div>
</template>


<style lang="scss" scoped>
.wt {
    width: 80%;  
    margin: 0 auto;
}
button {
    margin-top: 10px;
     background-color: #F5F5F5;
     padding: 5px;
    border: 2px solid #F5F5F5;
    border-radius: 2px;
    }
input {
     margin-top: 10px;
     background-color: #F5F5F5;
     padding: 5px;
     border: 2px solid #F5F5F5;
     border-radius: 2px;
    }


</style>