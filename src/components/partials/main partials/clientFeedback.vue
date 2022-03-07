<template>
    <section>
        <div class="feedback d-flex justify-content-center align-items-center flex-column">
            <h1>Client Feedback</h1>
            <littleRule class="mt-3"/>
        </div>
        <div class="clients row">

            <feedbackCard
            v-for="(review, index) in reviews" 
            :key="index"
            :cards="review"
            class="col-3 client-feedback d-flex flex-column align-items-center justify-content-center pt-4" 
            />

        </div>
    </section>
    
</template>

<script>
import littleRule from './littleRule.vue'
import feedbackCard from './feedbackCard.vue'


export default {
    name: 'clientFeedback',

    data(){
        return{

            reviews:[

                {
                    logo: require("../../../assets/img/client-logo-8-200x87.png"),
                    text: '"Avada Finance offers a fantastic service! It is easy to use and the customer support is the best around. This payment option is my number one choice. I always recommend it"',
                    name: 'ANDREA MENDOZA',
                    role: 'CREATIVE MARKET'
                },

                {
                    logo: require("../../../assets/img/client-logo-1-1-200x87.png"),
                    text: '"Avada Finance offers a fantastic service! It is easy to use and the customer support is the best around. This payment option is my number one choice. I always recommend it"',
                    name: 'ANDREA MENDOZA',
                    role: 'CREATIVE MARKET'
                },

                {
                    logo: require("../../../assets/img/client-logo-2-200x87.png"),
                    text: '"Avada Finance offers a fantastic service! It is easy to use and the customer support is the best around. This payment option is my number one choice. I always recommend it"',
                    name: 'ANDREA MENDOZA',
                    role: 'CREATIVE MARKET'
                },

                {
                    logo: require("../../../assets/img/client-logo-3-200x87.png"),
                    text: '"Avada Finance offers a fantastic service! It is easy to use and the customer support is the best around. This payment option is my number one choice. I always recommend it"',
                    name: 'ANDREA MENDOZA',
                    role: 'CREATIVE MARKET'
                }
            ]
        }
    },

    components:{
        littleRule,
        feedbackCard
    }
}
</script>

<style scoped lang="scss">
    @import '../../../assets/style/colorPalette.scss';
    @import '../../../assets/style/common.scss';

    
    .feedback{
        padding: 80px 0;
        background: $BlackHaze;
    }

    .clients{
        width: 100%;
        .client-feedback{
            border: solid $BlackHaze 1px;
        }
    }

</style>