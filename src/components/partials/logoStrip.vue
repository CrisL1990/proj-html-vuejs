<template>
    <section class="logoStrip row row-cols-6">
        <singleLogo v-for="(logo, index) in logos" :key="index" 
        class="col d-flex justify-content-center align-items-center h-100" 
        :logo="logo.filePath"
        />
    </section>
</template>

<script>

import singleLogo from './singleLogo.vue'

export default {
    name: 'logoStrip',

    components:{
        singleLogo
    },

    data(){
        return{

            logos:[

                {
                    filePath: require('../../assets/img/client-logo-7-200x87.png'),
                
                },

                {
                    filePath: require('../../assets/img/client-logo-8-200x87.png'),
          
                },

                {
                    filePath: require('../../assets/img/client-logo-9-200x87.png'),
           
                },

                {
                    filePath: require('../../assets/img/client-logo-5-200x87.png'),
                    
                },

                {
                    filePath: require('../../assets/img/client-logo-6-200x87.png'),
                 
                },

                {
                    filePath: require('../../assets/img/client-logo-7-200x87.png'),
                  
                }
            ]
        }
    }
}
</script>

<style scoped lang='scss'>
     @import "../../assets/style/colorPalette.scss";
     @import '../../assets/style/common.scss';

    .logoStrip{
        height: 150px;
        background-color: $BlackHaze;
        width: 100%;
        
    }
</style>