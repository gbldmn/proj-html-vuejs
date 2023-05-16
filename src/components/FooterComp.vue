<script>

export default {
    name: "FooterComp.vue",
    props: {
        footerMenu: Array
    }
}

</script>


<!-- PARTE FINALE -->

<template>
<div class="box">
    <div class="box2 d-flex justify-content-between align-items-center">
        <div class="d-flex flex-column">
            <h5>Address</h5>
            <span>382 NE 191st St # 87394 Miami, FL 33179-3899</span>
            <span>+1 (305) 547-9909 (9am - 5pm EST, Monday-Friday)</span>
            <span>support@maxchoac.com</span>
            <span> <a href=""><i class="fa-brands fa-square-facebook"></i></a>  <a href=""> <i class="fa-brands fa-twitter"></i></a> <a href=""><i class="fa-brands fa-instagram"></i></a> <a href=""><i class="fa-brands fa-linkedin"></i></a>   </span>
        </div>
        <div class="d-flex align-items-end br">
           <span class="we"><i class="fa-regular fa-copyright"></i>2020 Maxchoac <strong>All Reserved</strong></span>
        </div>
        <div class="d-flex">
            <div v-for="(elemMenu, index) in footerMenu" :key="index">
                <h6>{{ elemMenu.nome }}</h6>
                <ul>
                    <li v-for="(elem, index) in elemMenu.subMenu" :key="index">
                     <a href="">{{ elem }}</a></li>
                </ul>
            </div>
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
.box {
    width: 100%;
    height: 500px;
    background-color: #F8F8F8;
}
.box2 {
    width: 70%;
    margin: 0 auto;
    height: 100%;
}
h6 {
    height: 20px;
}
ul li {
    list-style: none;
    list-style-position: inside;
    line-height: 2rem;
}
span {
    line-height: 2.5rem;
}
i {
    margin-right: 1rem;
    font-size: 20px;
}
h6 {
    margin-left: 27px;
}
a {
    color: #333333;
    text-decoration: none;
}
.br {
    height: 350px;
    width: 250px;
}
.we {
    color: #ABABAB;
}
</style>