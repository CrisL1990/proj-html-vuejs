<template>
    <div class="col py-5">

        <h6>{{menu[2].title}}</h6>

        <ul>
            <li>
               <a href="#"><i :class="menu[2].icon"></i></a> 
            </li>
        </ul>

    </div>
</template>

<script>
export default {
    name: 'footerMenuBox3',

    props:{

        'menu': Object
    }
}
</script>

<style scoped lang="scss">
    @import '../../../assets/style/colorPalette.scss';  
    @import '../../../assets/style/footerTopBox.scss';

    .fa-twitter{
        color: $Blue;
        font-size: 20px;
    }
</style>