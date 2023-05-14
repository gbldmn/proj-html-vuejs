<script>

import SearchComp from './components/SearchComp.vue'
import MainComp from './components/MainComp.vue'
import MainComp2 from './components/MainComp2.vue'
import MainComp3 from './components/MainComp3.vue'
import MainComp4 from './components/MainComp4.vue'
import FooterComp from './components/FooterComp.vue'
import PrefooterComp from './components/PrefooterComp.vue'


export default {
    name: "app",
    components: {
        SearchComp,
        MainComp,
        MainComp2,
        MainComp3,
        MainComp4,
        FooterComp,
        PrefooterComp
    },
    data() {
        return {
            menu: [
                {
                    nome: 'home',
                    subMenu:[
                        'Subscribe',
                        'Enter',
                        'News',
                    ]
                },
                {
                    nome: 'Pages',
                    subMenu:[
                        'Maxchoach',
                        'componiorship',
                        'Featured',
                    ]
                },
                {
                    nome: 'Courses',
                    subMenu:[
                        'works'
                    ]
                },
                {
                    nome: 'Features',
                    subMenu:[
                        'Menu',
                        'Documentation',
                        'support'

                    ]
                },
                {
                    nome: 'blog',
                    subMenu:[
                        ' List',
                        ' Grid',
                        ' Type'
                    ]
                },
                {
                    nome: 'Shop',
                    subMenu:[
                        'My Shop',
                        'Card',
                        'Whishlist'

                    ]
                },
                
            ],
            footerMenu: [
                {
                    nome: 'Explore',
                    subMenu:[
                        'Start here',
                        'Blog',
                        'About us',
                    ]
                },
                {
                    nome: '',
                    subMenu:[
                        'Success Story',
                        'Courses',
                        'Contact us',
                    ]
                },
                {
                    nome: 'Information',
                    subMenu:[
                        'Membership',
                        'Purchase guide',
                        'Privacy policy',
                        'Terms of services'
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
    <PrefooterComp/>
    <FooterComp :footerMenu="footerMenu"/>
</main>
  
</template>

<style lang="scss">
@use './style/main.scss';


</style>
