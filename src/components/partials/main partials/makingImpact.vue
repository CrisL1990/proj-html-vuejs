<template>
    <section class="impact d-flex justify-content-between">
        
        <div class="box-left d-flex flex-column justify-content-center px-5">
            <span class="my-4">Investment Numbers</span>
            <h1>Making An Impact In Our Communities</h1>
            <button class="my-4"> <a href="#">LEARN MORE</a> </button>
        </div>

        <div class="box-right d-flex align-items-center justify-content-center">

            <div class="percentage-container">

                <boxPercentage v-for="(statistic, index) in statistics" :key="index"
                class="box d-flex flex-column justify-content-center align-items-center pe-5 pb-5"
                :statistics="statistic"
                />

            </div>
        
        </div>

    </section>
</template>

<script>

    import boxPercentage from './boxPercentage.vue'
    export default {
        name:'makingImpact',

        components:{
            boxPercentage
        },

        data(){

            return{

                statistics: [
                    {
                        percentage: "86%",
                        text: "Succesful Applications"
                    },

                    {
                        percentage: "94%",
                        text: "Return On Investment"
                    },

                    {
                        percentage: "92%",
                        text: "Applied Solutions"
                    },

                    {
                        percentage: "100%",
                        text: "Completely Secure"
                    },
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
    @import "../../../assets/style/colorPalette.scss";
    @import "../../../assets/style/roundedButton.scss";    
    @import '../../../assets/style/common.scss'; 
    
    .impact{
        height: 500px;
        
        .box-left{
            height: 100%;
            width: 35%;
            background-image: url('../../../assets/img/counters-bg-image.jpg');
            background-size: cover;
            color: $White;
        }
        .box-right{
            height: 100%;
            width: 60%;

            .percentage-container::after{
                content: "";
                clear: both;
                display: table;
            }
            
                .box{
                    height: 100%;
                    width: 50%;
                    float: left; 
                }
            }
        }

        button{
            padding: $padding;
            width: 150px;
            border-radius: $border-radius30;
            color: $White;
            background-color: $Water;
            font-weight: bold;
            border: none;
            font-size: $button-font-zize;
            
            a{
                text-decoration: none;
                color: $White;
            }
        }
    
</style>