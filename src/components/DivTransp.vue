<template>
    <div class="item">
        <div class="containerTrans">
            <div class="headingBlocks">
                <h1>Наш транспорт</h1>
            </div>
            <div class="info-transport">
                <div class="our-car"></div>
                <div class="info-car">
                    <div class="mass-car">
                        <p>Грузоподъемность 2 тонны</p>
                    </div>
                    <div class="name-car">
                        <p>Mercedes Sprinter</p>
                    </div>
                </div>
            </div>
            <div class="full-description-car">
                <ul>
                    <li>Длина кузова <span class="valueDesc">3,30</span> метра </li>
                    <li>Цельнометаллический фургон</li>
                    <li>Ширина <span class="valueDesc">1,70</span> метра </li>
                    <li>Высота <span class="valueDesc">1,80</span> метра </li>
                </ul>
            </div>
            <br>
        </div>
    </div>
</template>

<script>
export default {
  name: 'DivTransp'
}
</script>

<style scoped>
    .containerTrans{
        position: relative;
        background-color: chocolate;
    }
    .info-transport{
        display: flex;
        justify-content: center;
    }
    .our-car{
        width: 400px;
        height: 220px;
        background: url("../assets/picture/MersSprinter-v3.jpg") no-repeat center center ;
        background-size: cover;
        display: inline-block;
        margin: 5px;
        animation: our-car 10s infinite alternate-reverse;
    }

    .info-car{
        display: block;
    }
    .mass-car, .name-car, .our-car{
        -webkit-border-radius: 5px;
        -moz-border-radius: 5px;
        border-radius: 5px;
        padding: 10px;
    }
    .mass-car, .name-car{
        width: 300px;
        height: 100px;
        margin: 5px;
        margin-left: 20px;
        text-align: center;
        background-color: rgb(255, 207, 145);
        box-shadow: 5px 5px 5px black;
        border-style: solid;
        -webkit-transform: skew(-10deg);
        -moz-transform: skew(-10deg);
        -o-transform: skew(-10deg);
        border-radius: 10px;
    }
    .mass-car{
        margin-bottom: 20px;
    }
    .name-car{
        margin-top: 20px;
        padding-top: 30px;
        padding-left: 5px;
    }

    .mass-car, .name-car p{
        font-size: 28px;
        font-weight: bolder;
    }
    li{
        list-style-image: url("../assets/picture/car_wheel.png");
    }
    .full-description-car{
        margin: 15px;
        margin-left: 25px;
        font-size: 24px;
    }
    .valueDesc{
        font-weight: bold;
        font-size: 26px;

    }

    @media screen and (max-width: 425px) and (max-width: 375px) {
        .info-transport{
            display: block;
        }
        .info-car{
            display: flex;
            justify-content: center;
        }

    }

    @media screen and (max-width: 425px) {
        .info-transport{
            display: block;
        }
        .info-car{
            display: flex;
            justify-content: center;
        }
        .our-car{
            width: 415px;
            height: 250px;

        }
        .mass-car, .name-car p{
            font-size: 19px;
            margin-left: 10px;
        }
        .mass-car, .name-car{
            margin: 15px;
            width: 200px;
            height: 75px;
        }
        .name-car{
            padding-top: 10px;
        }
        .full-description-car{
            font-size: 18px;
            margin-top: 15px;
            margin-left: 0;
        }
        .valueDesc{
            font-size: 24px;
        }
    }

    @media screen and (max-width: 376px){
        .our-car{
            width: 365px;
            height: 200px;

        }
        .mass-car, .name-car p{
            font-size: 16px;
        }

        .name-car p{
            font-size: 18px;
            padding-top:5px;
        }
        .full-description-car{
            font-size: 18px;
            margin-top: 15px;
            margin-left: 0;
        }
        .valueDesc{
            font-size: 24px;
        }
    }
</style>
