<template>
    <section class="footer-top row row-cols-4">

        <div class="col logo-container pt-5 px-5">
            <a href="#"><img class="w-50" src="../../../assets/img/finance_logo_footer-200x131.png" alt=""></a> 
        </div>

        <footerMenuBox1 :menu="links"/>
        <footerMenuBox2 :menu="links"/>
        <footerMenuBox3 :menu="links"/>
        
    </section>
</template>

<script>

import footerMenuBox1 from './footerMenuBox1.vue'
import footerMenuBox2 from './footerMenuBox2.vue'
import footerMenuBox3 from './footerMenuBox3.vue'

export default {
    name: 'footerTop',

    components:{
        footerMenuBox1,
        footerMenuBox2,
        footerMenuBox3
    },

    data(){

        return{

            links:[
                {   
                    title: 'RECENT POSTS',
                    options: [

                        {
                            icon: 'fa-solid fa-angle-right me-2',
                            link: 'When is it the right time to sell your company?'
                        },

                        {
                            icon: 'fa-solid fa-angle-right me-2',
                            link: 'Personal debt or company debt we explore your options'
                        },

                        {
                            icon: 'fa-solid fa-angle-right me-2',
                            link: 'An interview with a so-called business angel'
                        }
                    ]
                },

                {
                    title: 'SERVICES',
                    options: [

                        {
                            icon: 'fa-solid fa-angle-right me-2',
                            link: 'SMALL BUSINESS LOANS SERVICES'
                        },

                        {
                            icon: 'fa-solid fa-angle-right me-2',
                            link: 'CREDIT RATING ADVICE SERVICES'
                        },

                        {
                            icon: 'fa-solid fa-angle-right me-2',
                            link: 'CROWD FOUNDING SERVICES'
                        }
                    ]
                },
                
                {
                    title: 'LATEST',
                    icon: 'fa-brands fa-twitter mt-2'
                }

            ]
        }
    }
}
</script>

<style scoped lang="scss">

    @import '../../../assets/style/colorPalette.scss';

    .footer-top{
        background-color: $balticSea; 
    }

</style>