<template>
    <section>
        <div class="jumbotron d-flex justify-content-center align-items-center">
            <h1>Right people<span>. </span>Right Investments<span>.</span></h1>
        </div>
    </section>
</template>

<script>
export default {
    name: 'myJumbotron'
}
</script>

<style scoped lang="scss">

    @import "../../assets/style/colorPalette.scss";
    @import '../../assets/style/common.scss';

    .jumbotron{
        background-image: url('../../assets/img/home_finance_slider_bg.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        width: 100%;
        height: 800px;

        h1{
            color: $White;
            font-size: 60px;

            span{
                color: $Blue;
            }
        }
    }
</style>