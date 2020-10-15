<template>
    <div class="item">
        <div class="headingBlocks">
            <h1>Способ оплаты</h1>
        </div>
        <div class="list-payment">
            <ul>
                <li>Наличный расчет</li>
                <li>Без наличный расчет</li>
            </ul>
        </div>
        <br>
    </div>
</template>

<script>
import DivOppSale from './DivOppSale'
export default {
  name: 'typePayment',
  // eslint-disable-next-line vue/no-unused-components
  components: { DivOppSale }
}
</script>

<style scoped>
    .list-payment{
        width: 95%;
        border: 5px black solid;
        background-color: rgb(255, 207, 145);
        margin: 0 auto;
    }

    li{
        margin: 10px;
        margin-left: 20px;
        list-style-image: url("../assets/picture/car_wheel.png");
        font-size: 28px;
    }

    @media screen and (max-width: 375px) {
        ul{
            padding-left: 30px;
        }
        li{
            margin-left: 0;
            font-size: 20px;
        }
    }
</style>
