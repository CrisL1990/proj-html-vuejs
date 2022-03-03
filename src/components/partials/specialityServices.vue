<template>
    <div class="section-cont"> 
        <div class="wrapper">
            <section class="speciality d-flex flex-column align-items-center justify-content-center">
                <h1 class="my-3">Speciality Services</h1>
                <littleRule />
                <p class="text-center my-4">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vitae mollitia, eum explicabo dolore eaque nostrum iste recusandae. Dolore voluptas, sunt dolor nulla enim consequuntur tempore eaque, et ut, eligendi ipsum?</p>

                <div class="card text-center my-5">
                  
                    <i class="fa-solid fa-globe my-3"></i>
                    
                    <h5>Small Business Loans</h5>

                    <p class="my-2 mx-3">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates sed corrupti pariatur, magnam quibusdam error excepturi nostrum at.</p>

                    <button><a href="#">LEARN MORE</a></button>

                </div>
            </section>
        </div>
    </div>
    
    
</template>

<script>

import littleRule from './littleRule.vue'
export default {
    name: 'specialityServices',

    data(){
        return{
          
        }
    },

    components:{
        littleRule
    }
}
</script>

<style scoped lang="scss">
    @import "../../assets/style/colorPalette.scss";

    .section-cont{
        background-color: $BlackHaze;

        .wrapper{
            width: 70%;
            margin: auto;

            .speciality{
                
                height: 650px;

                .card{
                    max-width: 250px;
                    border: none;

                    i{
                        font-size: 40px;
                        color: $icon;
                    }

                    p{
                        font-size: 13px;
                        color: $gray;
                    }

                    button{
                        border: none;
                        background-color: $Water;
                        margin-top: 30px;
                        

                        a{
                            text-decoration: none;
                            color: $White;
                        }
                    }
                }
        
            }
        }
    }
    
    
</style>