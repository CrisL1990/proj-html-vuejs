<template>
    <div class="container d-flex justify-content-center align-items-center">
        <a href="#"><i :class="icons.social"></i></a>    
    </div>
</template>

<script>
export default {
    name: 'socialIcons',

    props:{
        
        'icons': Object
    }
}
</script>

<style scoped lang="scss">
    @import '../../../assets/style/colorPalette.scss';  

    .container{
        height: 30px;
        width: 30px;
        border-radius: 50%;
        background-color: $Water;

        i{
            color: $White;
        }
    }
</style>