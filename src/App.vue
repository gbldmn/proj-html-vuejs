<script>

import SearchComp from './components/SearchComp.vue'
import MainComp from './components/MainComp.vue'
import MainComp2 from './components/MainComp2.vue'
import MainComp3 from './components/MainComp3.vue'
import MainComp4 from './components/MainComp4.vue'


export default {
    name: "app",
    components: {
        SearchComp,
        MainComp,
        MainComp2,
        MainComp3,
        MainComp4,
    }
}

</script>

<template>
<header class="dab">
    <SearchComp/>
</header>
<main>
    <MainComp/>
    <MainComp2/>
    <MainComp3/>
    <MainComp4/>
</main>
  
</template>

<style lang="scss">
@use './style/main.scss';


</style>
