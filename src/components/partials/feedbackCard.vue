<template>
    <div>
        <div>
            <div class="d-flex justify-content-center">
                <img class="client-logo" :src="cards.logo" alt="Client logo">
            </div>

            <p class="review text-center px-4 mb-5"> 
                {{cards.text}}
            </p>
        </div>
                    
        <div class="client-name text-center">
            <p class="name pt-3">{{cards.name}}</p>
            <p class="role">{{cards.role}}</p>
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

    .client-logo{
        filter: brightness(0) invert(0);
    }

    .review{
        font-size: 13px;
        color: $gray;
    }

    .client-name{
        width: 100%;
        border-top: solid $BlackHaze 2px ;

        .name{
            line-height: 5px;
        }

        .role{
            font-size: 10px;
        }
    }  
</style>