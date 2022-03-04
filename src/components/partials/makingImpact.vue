<template>
    <section class="impact d-flex justify-content-between">
        
        <div class="box-left d-flex flex-column justify-content-center px-5">
            <span class="my-4">Investment Number</span>
            <h1>Making An Impact In Our Communities</h1>
            <button class="my-4"> <a href="#">LEARN MORE</a> </button>
        </div>

        <div class="box-right">

            <div class="row row-cols-2 pt-5">

                <div class="col box d-flex flex-column justify-content-center align-items-center">
                    <h1>86%</h1>
                    <p>Succesful Applications</p>
                </div>

                <div class="col box d-flex flex-column justify-content-center align-items-center">
                    <h1>94%</h1>
                    <p>Return On Investment</p>
                </div>

            </div>

            <div class="row row-cols-2 pb-5">

                <div class="col box d-flex flex-column justify-content-center align-items-center">
                    <h1>92%</h1>
                    <p>Applied Solutions</p>
                </div>

                <div class="col box d-flex flex-column justify-content-center align-items-center">
                    <h1>100%</h1>
                    <p>Completely Secure</p>
                </div>

            </div>

        </div>

    </section>
</template>

<script>
export default {

    name:'makingImpact'

}
</script>

<style scoped lang="scss">

    @import "../../assets/style/colorPalette.scss";
    @import "../../assets/style/roundedButton.scss";     

    .impact{
        width: 100%;
        height: 500px;
        

        .box-left{
            height: 100%;
            width: 35%;
            background-image: url('../../assets/img/counters-bg-image.jpg');
            background-size: cover;
            color: $White;
        }

        .box-right{
            height: 100%;
            width: 60%;
            
            .row{
                height: 50%;

                .col{

                    h1{
                        color: $icon;
                    }

                    p{
                        font-size: 10px;
                    }
                }
            }
        }

        button{
            padding: $padding;
            width: 150px;
            border-radius: $border-radius30;
            color: $White;
            background-color: $Water;
            font-weight: bold;
            border: none;

            a{
                text-decoration: none;
                color: $White;
            }
        }
    }

</style>