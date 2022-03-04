<template>
    <div>       
        <i :class="cardInfo.icon"></i>
        <h5>{{cardInfo.title}}</h5>
        <p class="my-2 mx-3">{{cardInfo.par}}</p>
        <button><a href="#">{{cardInfo.button}}</a></button>
    </div>  
</template>

<script>
export default {    
    name: 'servicesCard',

    props:{

        'cardInfo': Object
    }
}
</script>

<style scoped lang="scss">

    @import "../../assets/style/colorPalette.scss";

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
        width: 100%;
                
        a{
            text-decoration: none;
            color: $White;
        }
    }
    

</style>