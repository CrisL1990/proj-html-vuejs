<template>
    <header class="row">

        <div class="col-4 d-flex align-items-center px-5 img-cont">
            <img src="../assets/img/finance_logo_1x.png" alt="">
        </div>

        <div class="col-8 d-flex justify-content-end px-5 align-items-center">

            <navList :menuVoices="navVoices"/>
            <!--
            <ul class="d-flex align-items-center">
                <li>
                    <a href="#">HOME</a>
                </li>
                <li>
                    <a href="#">ABOUT</a>
                </li>
                <li>
                    <a href="#">SERVICES</a>
                </li>
                <li>
                    <a href="#">PACKAGES</a>
                </li>
                <li>
                    <a href="#">INSIGHT</a>
                </li>
                <li>
                    <button><a href="#">CONTACT</a></button>
                </li>
                <li>
                    <a href="#">+</a>
                </li>
            </ul>
            -->
        </div>
        
    </header>
</template>

<script>
import navList from './partials/header partials/navList.vue'
export default {

    name: 'myHeader',

    components:{
        navList
    },

    data(){
        return{

            navVoices:[

                {
                    link: 'HOME'
                },

                {
                    link: 'ABOUT'
                },

                {
                    link: 'SERVICES'
                },

                {
                    link: 'PACKAGES'
                },

                {
                    link: 'INSIGHT'
                },

                {
                    link: 'CONTACT'
                },

                {
                    link: '+'
                },
            ]
            
        }
    }

}
</script>

<style scoped lang="scss">

    @import './../assets/style/colorPalette.scss';
    @import './../assets/style/roundedButton.scss';

    header{

        height: 80px;
        width: 100%;

        .col-4, .col-8{
            height: 100%;
        }

        .img-cont{

            img{
                width: 50%;
            }
        }
    }
</style>