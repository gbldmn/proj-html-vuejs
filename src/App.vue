<script>

import SearchComp from './components/SearchComp.vue'
import MainComp from './components/MainComp.vue'


export default {
    name: "app",
    components: {
        SearchComp,
        MainComp
    }
}

</script>

<template>
<header class="dab">
    <SearchComp/>
</header>
<main>
    <MainComp/>
</main>
  
</template>

<style lang="scss">
@use './style/main.scss';


</style>
