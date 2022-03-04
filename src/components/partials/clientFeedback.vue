<template>
    <section class="feedback d-flex justify-content-center align-items-center flex-column">
        <h1>Client Feedback</h1>
        <littleRule class="mt-3"/>
    </section>
</template>

<script>
import littleRule from './littleRule.vue'
export default {
    name: 'clientFeedback',

    components:{
        littleRule
    }
}
</script>

<style scoped lang="scss">
    @import '../../assets/style/colorPalette.scss';

    .feedback{
        height: 250px;
        width: 100%;
        background: $BlackHaze;
    }

</style>