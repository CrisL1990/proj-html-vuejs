<template>
    <div>
        <div>
            <div class="d-flex justify-content-center">
                <img class="client-logo" :src="cards.logo" alt="Client logo">
            </div>

            <p class="review text-center px-5 mb-5"> 
                {{cards.text}}
            </p>
        </div>
                    
        <div class="client-name text-center">
            <p class="name mt-3 py-2">{{cards.name}}</p>
            <p class="role pb-3">{{cards.role}}</p>
        </div>
    </div>
    
</template>

<script>

export default {
    name: 'feedbackCard',

    props:{
        'cards': Object
    }
}
</script>

<style scoped lang="scss">
    @import '../../assets/style/colorPalette.scss';
    @import '../../assets/style/common.scss';

    .client-logo{
        filter: brightness(0) invert(0);
    }

    .review{
        font-size: 15px;
        color: $gray;
        font-family: 'Frank Ruhl Libre', serif;
    }

    .client-name{
        width: 100%;
        border-top: solid $BlackHaze 2px ;

        .name{
            line-height: 5px;
            font-size: 12px;
            font-weight: bold;
        }

        .role{
            font-size: 10px;
            color: $gray;
        }
    }  
</style>