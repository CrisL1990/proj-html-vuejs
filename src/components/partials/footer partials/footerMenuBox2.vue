<template>
    <div class="col py-5">

        <h6>{{menu[1].title}}</h6>

        <ul>
            <li v-for="(item, index) in menu[1].options" :key="index">
                <i :class="item.icon"></i>
                <a href="#">{{item.link}}</a> 
            </li>
        </ul>

    </div>
</template>

<script>
export default {
    name: 'footerMenuBox2',

    props:{

        'menu': Object
    }
}
</script>

<style scoped lang="scss">
    @import '../../../assets/style/colorPalette.scss';  
    @import '../../../assets/style/footerTopBox.scss';
    @import '../../../assets/style/common.scss';
</style>