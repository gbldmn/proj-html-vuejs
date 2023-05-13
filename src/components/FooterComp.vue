<script>

export default {
    name: "FooterComp.vue",
    props: {
        footerMenu: Array
    }
}

</script>

<template>
<div class="box">
    <div class="box2 d-flex justify-content-between align-items-center">
        <div class="d-flex flex-column">
            <h6>address</h6>
            <span>fffffffff</span>
            <span>gggggggg</span>
            <span>rrrrrrrrr</span>
            <span>ggggggg</span>
        </div>
        <div class="d-flex">
            <div v-for="(elemMenu, index) in footerMenu" :key="index">
                <h6>{{ elemMenu.nome }}</h6>
                <ul>
                    <li v-for="(elem, index) in elemMenu.subMenu" :key="index">
                        {{ elem }}</li>
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
}
.box2 {
    width: 80%;
    margin: 0 auto;
    height: 100%;
}
h6 {
    height: 20px;
}
</style>