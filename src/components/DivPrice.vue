<template>
    <div class="item">
        <div class="headingBlocks">
            <h1>Наши цены</h1>
        </div>
        <div class="priceList">
            <div class="hourPrice">
                <div class="inMinsk">
                    <div class="price">от <b>17</b> <span class="money">BYN</span></div>
                    <div class="termsPrice">За час работы в Минске</div>
                </div>
                <div class="notinMinsk">
                    <div class="price mb-4">от <b>0,5</b> <span class="money">BYN</span></div>
                    <div class="termsPrice mb-4">За 1 км работы за МКАД</div>
                </div>
            </div>
        </div>
        <br>
    </div>
</template>

<script>
export default {
  name: 'DivPrice'
}
</script>

<style>

    .inMinsk, .notinMinsk{
        display: flex;
    }
    .price, .termsPrice{
        font-size: 35px;
        min-width: 300px;
        max-width: 450px;
        max-height: 70px;
        -webkit-transform: skew(-20deg);
        -moz-transform: skew(-20deg);
        -o-transform: skew(-20deg);
        border-style: solid;
        margin: 0 auto;
        border-radius: 10px;
        box-shadow: 10px 10px 5px rgba(0, 0, 0, 1);
        padding: 10px;
        text-align: center;
        margin-bottom: 30px;
        /*animation: price 1s linear infinite alternate;*/
    }

    .price{
        background-color: rgb(255, 207, 145);
        padding-top: 10px;
    }
    .termsPrice{
        background-color: chocolate;
    }

    @media screen and (max-width: 425px) {
        .price, .termsPrice {
            font-size: 25px;
            font-weight: bold;
            min-width: 50px;
            max-width: 210px;
            max-height: 80px;
        }
        .price{
            padding-top: 20px;
        }
        .termsPrice{
            padding-top: 5px;
        }
    }
    @media screen and (max-width: 376px) {
        .termsPrice {
            font-size: 18px;
            min-width: 50px;
            max-width: 150px;
            max-height: 80px;
            padding: 10px;
        }
        .price{
            padding-top: 15px;
        }
    }

</style>
