<template>
    <div class="wrapper">
        <section class="cloud-cont row row-cols-2">

            <div class="col d-flex justify-content-center align-items-start flex-column">
                <h1 class="my-4">Cloud Based Finance</h1>
                <littleRule class="my-2" />

                <p class="my-4">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Rerum et illo explicabo distinctio  nemo quidem, quae eos cum. Error!</p>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptas distinctio quaerat repudiandae consequuntur a voluptatibus eum, eveniet voluptatum officia eligendi dignissimos?</p>
               
                <button class="my-4">LEARN MORE</button>
            </div>

            <div class="col d-flex justify-content-center align-items-start flex-column px-5">
                <img src="../../assets/img/graph-600x457.jpg" alt="">
            </div>

        </section>
    </div>
    
</template>

<script>

import littleRule from './littleRule.vue'
export default {
    name: 'cloudBased',

    components:{
        littleRule,
    }


}
</script>

<style scoped lang="scss">

    @import '../../assets/style/roundedButton.scss';
    @import '../../assets/style/colorPalette.scss';

    .wrapper{
        width: 80%;
        margin: auto;

        .cloud-cont{
        width: 100%;
        height: 500px;
        }

        button{
            padding: $padding;
            width: 150px;
            border-radius: $border-radius30;
            color: $White;
            background-color: $Water;
            font-weight: bold;
            border: none;
        }
    }
    

</style>