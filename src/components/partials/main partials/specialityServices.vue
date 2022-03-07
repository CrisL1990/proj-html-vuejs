<template>
    <div class="section-cont"> 
        <div class="wrapper">
            <section class="speciality d-flex flex-column align-items-center justify-content-center">
                <h1 class="my-3">Specialty Services</h1>
                <littleRule />
                <p class="text-center my-4 par">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vitae mollitia, eum explicabo dolore eaque nostrum iste recusandae. Dolore voluptas, sunt dolor nulla enim consequuntur tempore eaque, et ut, eligendi ipsum?</p>

                <div class="d-flex justify-content-center">
                    
                    <servicesCard class="single-card text-center my-5" 
                    v-for="(card, index) in cards" :key="index" 
                    :cardInfo="card"
                    />

                </div>
            </section>
        </div>
    </div>
    
    
</template>

<script>

import littleRule from './littleRule.vue'
import servicesCard from './servicesCard.vue'

export default {
    name: 'specialityServices',

    data(){
        return{

            cards:[

                {
                    icon: 'fa-solid fa-globe my-3',
                    title: 'Small Business Loans',
                    par: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates sed corrupti pariatur, magnam quibusdam error excepturi nostrum at.',
                    button: 'Learn More'
                },

                {
                    icon: 'far fa-gem my-3',
                    title: 'Credit Rating Advice',
                    par: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates sed corrupti pariatur, magnam quibusdam error excepturi nostrum at.',
                    button: 'Learn More'
                },

                {
                    icon: 'fa fa-chart-line my-3',
                    title: 'Fast Crowd Founding',
                    par: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates sed corrupti pariatur, magnam quibusdam error excepturi nostrum at.',
                    button: 'Learn More'
                }
            ]
          
        }
    },


    components:{
        littleRule,
        servicesCard
    }
}
</script>

<style scoped lang="scss">

    @import "../../../assets/style/colorPalette.scss";

    .section-cont{
        background-color: $BlackHaze;

        .wrapper{
            padding: 80px 0;
            width: 70%;
            margin: auto;

            .speciality{

                .par{
                    font-size: 13px;   
                    color: $gray;  
                    padding: 0 250px; 
                }
                
                .single-card{
                    margin: 0 15px;
                    width: calc(100% / 3 - 90px);
                    max-width: 320px;
                    background-color: $White;
                    border: none;
                }
        
            }
        }
    }
    
    
</style>