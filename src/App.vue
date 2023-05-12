<script>

import SearchComp from './components/SearchComp.vue'
import MainComp from './components/MainComp.vue'
import MainComp2 from './components/MainComp2.vue'


export default {
    name: "app",
    components: {
        SearchComp,
        MainComp,
        MainComp2
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
</main>
  
</template>

<style lang="scss">
@use './style/main.scss';


</style>
