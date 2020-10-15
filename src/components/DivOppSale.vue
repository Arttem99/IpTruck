<template>
    <div class="item">
        <div class="content">
            <div class="headingBlocks">
                <h1>Возможность приобрести</h1>
            </div>
            <div class="container-opp">
                <div class="list-opportunities">
                    <ul>
                        <li><h4>Песок (2 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Песок плывун (2 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Гравий (2,5 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Щебень гравийный (3,5 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Торф (3,5 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Грунт (3,5 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Асфальтная крошка (3,5 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Щебень гранитный (5 <span class="money">BYN</span>)</h4></li>
                        <li><h4>Торфогрунт (6 <span class="money">BYN</span>)</h4></li>
                    </ul>
                </div>
                <div class="delivery-method">
                    <div class="info-dost"><p>Доставка в мешках</p></div>
                    <div class="pic-bag"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'DivOppSale'
}
</script>

<style scoped>
    h1{
        line-height: 1em;
    }
    .content{
        margin: 0px auto;
    }
    .container-opp{
        display: flex;
        justify-content: center;
    }
    .list-opportunities{
        border: 5px solid;
        width: 500px;
        background-color: rgb(255, 207, 145);
        font-size: 28px;
        margin-right: 10px;
    }
    ul{
        margin-top: 20px;
        margin-left: 20px;
    }
    .info-dost{
        margin-top: 15px;
        margin-bottom: 20px;

    }
    .delivery-method{
        width: 250px;
        border: 5px solid;
        background-color: #FF9A40;
        font-size: 34px;
        text-align: center;
        font-weight: bold;

    }
    .pic-bag{
        margin: 0 auto;
        background: url("../assets/picture/bag.png") no-repeat center center;
        background-size: cover;
        width: 170px;
        height: 190px;
    }
    li{
        list-style-image: url("../assets/picture/car_wheel.png");
    }

    @media screen and (max-width: 425px) {
        .container-opp{
            display: block;
            justify-content: center;
        }

        .list-opportunities{
            width: 425px;
            font-size: 25px;
        }
        .delivery-method{
            width: 425px;
            margin-top: 5px;
            padding-bottom: 10px;
        }
    }
    @media screen and (max-width: 375px){

        .container-opp{
            justify-content: center;
        }
        .list-opportunities{
            width: 375px;
            border: 5px solid;
            font-size: 25px;

        }
        .delivery-method{
            width: 375px;
            border: 5px solid;
            font-size: 25px;
        }
        .pic-bag{
            margin: auto;
            width: 130px;
            height: 145px;
        }
        ul{
            margin-top: 20px;
            margin-left: 15px;
            padding: 15px;
        }

        .info-dost{
            margin-top: 15px;
        }

    }

</style>
