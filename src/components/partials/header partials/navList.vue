<template>
    <nav>
        <ul class="d-flex align-items-center">
            <li v-for="(voice, index) in menuVoices" :key="index">
                <a class="active" v-if="voice.link != 'CONTACT'" href="#">{{voice.link}}</a>
                <button v-else><a href="#">{{voice.link}}</a></button>
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

    ul{
            height: 80px;
            margin-bottom: 0;

            li{
                display: flex;
                margin: 0 10px;
              
                height: 100%;
                align-items: center;

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
                        color: white;
                        
                    }
                }

                a{
                    text-decoration: none;
                    color: $gray;
                    font-size: 13px;
                    height: 100%;
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    padding: 0 10px;
                    
                }
            }
        }
</style>