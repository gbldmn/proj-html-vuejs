<script>

import SearchComp from './components/SearchComp.vue'
import MainComp from './components/MainComp.vue'
import MainComp2 from './components/MainComp2.vue'
import MainComp3 from './components/MainComp3.vue'
import MainComp4 from './components/MainComp4.vue'
import FooterComp from './components/FooterComp.vue'


export default {
    name: "app",
    components: {
        SearchComp,
        MainComp,
        MainComp2,
        MainComp3,
        MainComp4,
        FooterComp
    },
    data() {
        return {
            menu: [
                {
                    nome: 'home',
                    subMenu:[
                        'subMenu1',
                        'subMenu2',
                        'subMenu3',
                    ]
                },
                {
                    nome: 'Pages',
                    subMenu:[
                        'subMenu1',
                        'subMenu2',
                        'subMenu3',
                    ]
                },
                {
                    nome: 'Pages',
                    subMenu:[
           
                    ]
                },
                
            ],
            footerMenu: [
                {
                    nome: 'explore',
                    subMenu:[
                        'subMenu1',
                        'subMenu2',
                        'subMenu3',
                    ]
                },
                {
                    nome: '',
                    subMenu:[
                        'subMenu1',
                        'subMenu2',
                        'subMenu3',
                    ]
                },
                {
                    nome: 'informatio',
                    subMenu:[
                        'subMenu1',
                        'subMenu2',
                        'subMenu3',
                        'subMenu4'
                    ]
                }
            ]
        }
    }
}

</script>

<template>
<header class="dab">
    <SearchComp :menu="menu"/>
</header>
<main>
    <MainComp/>
    <MainComp2/>
    <MainComp3/>
    <MainComp4/>
    <FooterComp :footerMenu="footerMenu"/>
</main>
  
</template>

<style lang="scss">
@use './style/main.scss';


</style>
