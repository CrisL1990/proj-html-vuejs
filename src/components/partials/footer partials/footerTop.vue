<template>
    <section class="footer-top row row-cols-4">

        <div class="col logo-container pt-5 px-5">
            <img class="w-50" src="../../../assets/img/finance_logo_footer-200x131.png" alt="">
        </div>

        <div class="col py-5">
            <h6>RECENT POSTS</h6>

            <ul>
                <li>
                    <i class="fa-solid fa-angle-right me-2"></i>
                    <a href="#">When is it the right time to sell your company?</a> 
                </li>
                <li>
                    <i class="fa-solid fa-angle-right me-2"></i>
                    <a href="#">Personal debt or company debt we explore your options</a> 
                </li>
                <li>
                    <i class="fa-solid fa-angle-right me-2"></i>
                    <a href="#">An interview with a so-called business angel</a> 
                </li>
            </ul>
        </div>

        <div class="col py-5">
            <h6>SERVICES</h6>

            <ul>
                <li>
                    <i class="fa-solid fa-angle-right me-2"></i>
                    <a href="#">SMALL BUSINESS LOANS SERVICES</a> 
                </li>
                <li>
                    <i class="fa-solid fa-angle-right me-2"></i>
                    <a href="#">CREDIT RATING ADVICE SERVICES</a> 
                </li>
                <li>
                    <i class="fa-solid fa-angle-right me-2"></i>
                    <a href="#">CROWD FOUNDING SERVICES</a> 
                </li>
            </ul>
        </div>

        <div class="col py-5">
            <h6>LATEST</h6>
            <i class="fa-brands fa-twitter mt-2"></i>
        </div>

    </section>
</template>

<script>
export default {
    name: 'footerTop'
}
</script>

<style scoped lang="scss">

    @import '../../../assets/style/colorPalette.scss';

    .footer-top{
        background-color: $balticSea;
      

        .col{
            height: 100%;
        }

            h6{
                color: $White;
                margin-left: 32px;
            }

            ul{
                list-style: none;

                li{
                    margin: 10px 0;

                    i{
                        color: $gray;
                        font-size: 12px;
                    }

                    a{
                        text-decoration: none;
                        color: $gray;
                        font-size: 12px;
                    }
                }
            }

        .fa-twitter{
            color: $Blue;
            margin-left: 32px;
        }
        
    }

</style>