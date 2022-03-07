<template>
    <nav>
        <ul class="d-flex align-items-center">
            <li class="d-flex align-items-center" v-for="(voice, index) in menuVoices" :key="index">

                <a class="active d-flex align-items-center justify-content-center" 
                v-if="voice.link == 'SERVICES'" href="#">{{voice.link}} 
                    <i class="fa-solid fa-chevron-down ms-2"></i>
                </a>

                <a class="active d-flex align-items-center justify-content-center" 
                v-else-if="voice.link != 'CONTACT'" href="#">
                    {{voice.link}}
                </a>
                
                <button v-else>
                    <a href="#" class="d-flex align-items-center justify-content-center">{{voice.link}}</a>
                </button>
            </li>
        </ul>
    </nav>
</template>

<script>

export default {

    name:'navList',

    props:{

        'menuVoices': Object
    }



}
</script>

<style scoped lang='scss'> 
    @import '../../../assets/style/colorPalette.scss';
    @import '../../../assets/style/roundedButton.scss';
    @import '../../../assets/style/common.scss';

    ul{
            height: 80px;
            margin-bottom: 0;

            li{
                margin: 0 10px;
                font-family: 'Roboto', sans-serif;
                font-weight: 500;
                height: 100%;
          
                &:hover{
                    .active{
                        color: $Shark;
                        background-color: $BlackHaze;
                    }
                }
            
                button{
                    padding: $padding;
                    border-radius: $border-radius30;
                    border: none;
                    width: 120px;
                    height: 40px;
                    background-color: $Water;

                    a{
                        color: $BlackHaze;
                    }
                }

                a{
                    text-decoration: none;
                    color: $gray;
                    font-size: 13px;
                    height: 100%;
                    padding: 0 10px;

                    i{
                        font-size: 10px;
                    }
                    
                }
            }
        }
</style>