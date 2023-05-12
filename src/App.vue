<script>

import SearchComp from './components/SearchComp.vue'


export default {
    name: "app",
    components: {
        SearchComp
    }
}

</script>

<template>
<header>
    <SearchComp/>
</header>
  
</template>

<style lang="scss">
@use './style/main.scss';


</style>
