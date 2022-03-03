<template>
    <header class="row">

        <div class="col-4 d-flex align-items-center px-5 img-cont">
            <img src="../assets/img/finance_logo_1x.png" alt="">
        </div>

        <div class="col-8 d-flex">
        
        </div>
        
    </header>
</template>

<script>
export default {

    name: 'myHeader'

}
</script>

<style scoped lang="scss">
    header{

        height: 80px;
        width: 100%;

        .col-4, .col-8{
            height: 100%;
        }

        .img-cont{

            img{
                width: auto;
            }
        }
        
    }
</style>