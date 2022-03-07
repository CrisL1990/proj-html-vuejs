<template>
    <section class="footer-bottom d-flex px-5 justify-content-between align-items-center">
        <div>
            <span>Copiright 2012 - 2020 | Avada theme by Theme Fusion | All Rights Reserved | Powered by Wordpress</span>
        </div>
            
        <div class="d-flex">
            <socialIcons class="mx-1" v-for="(icon, index) in icons" :key="index" :icons="icon"/>
        </div>
    </section>
</template>

<script>

import socialIcons from './socialIcons.vue'
export default {
    name: 'footerBottom',

    data(){
        return{
            icons: [
                {
                    social: 'fa-brands fa-facebook-f'
                },

                {
                    social: 'fa-brands fa-twitter'
                },

                {
                    social: 'fa-brands fa-youtube'
                },

                {
                    social: 'fa-brands fa-instagram'
                }
            ]
        }
    },

    components:{
        socialIcons
    }


}
</script>

<style scoped lang="scss">
    @import '../../../assets/style/colorPalette.scss';
    @import '../../../assets/style/common.scss';
    

    .footer-bottom{
        height: 100px;
        background-color: $Shark;

        span{
            color: $gray;
            font-size: 10px;
        }
    }
</style>