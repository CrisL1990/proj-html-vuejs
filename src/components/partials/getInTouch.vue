<template>
    
        <section class="talk d-flex flex-column justify-content-center align-items-center">

            <div class="wrapper text-center">
                <h1>Ready to talk?</h1>
                <p class="my-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui sapiente eius incidunt natus delectus saepe perferendis fuga.!</p>
                <button><a href="#">LET'S TALK</a></button>
            </div>
            
        </section>
    
    
</template>

<script>

export default {
    name: 'getInTouch'
}
</script>

<style scoped lang="scss">

    @import '../../assets/style/roundedButton.scss';
    @import '../../assets/style/colorPalette.scss';

    
    
    .talk{
        width: 100%;
        height: 350px;
        background-image: url('../../assets/img/ready_to_talk_cta_bg.jpg');
        background-size: cover;

        .wrapper{
        width: 50%;
        margin: auto;
        }
        

        h1{
            color: $White;
        }

        p{
            color: $gray;
        }

        button{
            padding: $padding;
            border-radius: $border-radius30;
            background-color: $Water;
            border: none;
            width: 150px;

            a{
                text-decoration: none;
                color: $White;
            }
        }
    }
</style>