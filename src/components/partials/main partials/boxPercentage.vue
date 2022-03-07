<template>
    <div>
        <span>{{statistics.percentage}}</span>
        <p>{{statistics.text}}</p>
    </div>
</template>

<script>
export default {
    name:'boxPercentage',

    props:{

        'statistics': Object
    }
}   
</script>

<style scoped lang="scss">
    @import "../../../assets/style/colorPalette.scss";
    @import "../../../assets/style/roundedButton.scss";    
    @import '../../../assets/style/common.scss';

    span{
        color: $icon;
        font-size:50px;
    }

    p{
        font-size: 12px;
        color: $gray;
    }
</style>