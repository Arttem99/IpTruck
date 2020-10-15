<template>
    <div class="item">
        <div class="content">
            <div class="headingBlocks">
                <h1><b>У</b>слуги</h1>
            </div>
            <div class="list-services">
                    <div class="service"><p>Работаем с ТТН</p> <i class="fas fa-file-alt fa-2x icon-color"></i></div>
                    <div class="service cht"><p>Доставка по времени</p><i class="fas fa-stopwatch fa-2x icon-color"></i></div>
                    <div class="service"><p>Срочная доставка</p><i class="fas fa-shipping-fast fa-2x icon-color"></i></div>
                    <div class="service cht"><p>Погрузка / Разгрузка</p><i class="fas fa-truck-loading fa-2x icon-color"></i></div>
            </div>
            <br>
        </div>
    </div>
</template>

<script>
export default {
  name: 'DivServices'
}
</script>

<style scoped>
    .content{

        background-color: chocolate;
    }

    .headingBlocks{
        padding: 15px;
    }

    .list-services{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;

    }
    .service{
        margin: 20px;
        width: 325px;
        height: 150px;
        border: 5px solid;
        -webkit-transform: skew(-20deg);
        -moz-transform: skew(-20deg);
        -o-transform: skew(-20deg);
        border-radius: 10px;
        box-shadow: 5px 5px 5px black;
        font-size: 26px;
        text-align: center;
        margin-bottom: 20px;
        background-color: #fff;
    }
    .service p {
        margin: auto;
        margin-top: 35px;
        font-size: 30px;
        font-weight: bolder;
    }
    .icon-color{
        color: chocolate;
    }
    @media screen and (max-width: 425px){
        .service{
            margin: 10px;
            width: 250px;
            height: 120px;

        }
        .service p {
            margin: auto;
            margin-top: 20px;
            font-size: 25px;
            font-weight: bolder;
            padding: 10px;
        }
        .cht p{
            margin: 0;
        }
        .icon-color{
            font-size: 30px;

        }
    }
    @media screen and (max-width: 375px) {
        .service{
            margin-top: 5px;
        }

    }

</style>
