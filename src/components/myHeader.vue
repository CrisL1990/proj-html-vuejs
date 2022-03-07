<template>
    <header class="row">

        <!--Inizio logo-->
        <div class="col-4 d-flex align-items-center px-5 img-cont">
            <img src="../assets/img/finance_logo_1x.png" alt="">
        </div>
        <!--Fine logo-->

        <!--Inizio Nav-->
        <div class="col-8 d-flex justify-content-end px-5 align-items-center">
            <navList :menuVoices="navVoices"/>
        </div>
        <!--Fine Nav-->

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

            //Contiene la lista delle voci del nav
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

    //Importa settaggi per button e colori
    @import './../assets/style/colorPalette.scss';
    @import './../assets/style/roundedButton.scss';

    header{

        //Setta dimensione Header
        height: 80px;
        width: 100%;

        //Setta dimensione columns
        .col-4, .col-8{
            height: 100%;
        }

        //Setta dimensione logo
        .img-cont{
            img{
                width: 50%;
            }
        }
    }
</style>