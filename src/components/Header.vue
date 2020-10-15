<template>
    <div>
        <div class="containerHeader">
            <div id="frameName">
                <h1><span id="gryz"><b>Гр</b>узоперевозки</span></h1><h1><span id="bel"> по Беларуси</span></h1>
            </div>
            <div class="contacts">
                <i class="fa fa-phone-alt" aria-hidden="true"></i>
                <a href="tel:+375296587036"> +375 (29) 658-70-36</a>
                <br>
                <span> <i class="fa fa-clock"></i> Без выходных</span>
            </div>

        </div>
        <div class="containerPicture">
                <div class="road">
                    <div class="roadLine"></div>
                    <div class="car"></div>
                </div>

        </div>

    </div>
</template>

<script>

export default {
  name: 'Header'
}
</script>

<style scoped>
    h1{
        font-family: "Goose";
        /*line-height: 1em;*/
    }
a{
    text-decoration: none;
    color: black;
    text-shadow: 0 0 3px chocolate;
}
    .containerHeader{
        width: 100%;
        max-width: 450px;
        margin: 0 40px ;
    }

    #frameName{
        background-color: rgb(255, 207, 145);
        width: 100%;
        height: auto;
        -webkit-transform: skew(-20deg);
        -moz-transform: skew(-20deg);
        -o-transform: skew(-20deg);
        border-left:10px black double;
        border-bottom: 10px black double;
        border-right: 10px black double;
        text-align: right;
    }
    /*@media (max-width: 376px) {*/
    /*    #frameName{*/
    /*        width: 350px;*/
    /*        margin: 0;*/
    /*    }*/
    /*    #gryz{*/
    /*        font-size: 40px;*/
    /*    }*/
    /*    #bel{*/
    /*        font-size: 20px;*/
    /*    }*/
    /*}*/
    #gryz{
        /*font-family: 'mr_Insulag', sans-serif;*/
        font-size: 50px;
        margin-right: 5px;
    }

    #bel{
        font-size: 36px;
        margin: 10px 5px;
    }

    .contacts{
        text-align: right;
        margin: 10px;
        font-size: 24px;
    }
    @keyframes pulsate{
        50%{
            color: #000000;
            text-shadow:0 -1px rgba(0,0,0,.3),0 0 5px #f03000,0 0 8px chocolate;
        }
    }
    .contacts a{
        -webkit-animation: pulsate 1.2s linear infinite;
        animation: pulsate 1.2s linear infinite;
    }
    .contacts i {
        font-size: 30px;
    }

    .containerPicture{
        width: 100%;

    }
    .containerPicture:before{
        content: "";
        width: 100%;
        height: 30px;
        background: linear-gradient(180deg, rgba(235, 164, 121, 0.1), rgb(235, 164, 121) 25%);
        display: block;
        /*box-shadow: chocolate 10p;*/
    }
    .road{
        height: 100px;
        width: 100%;
        background-color: #636b6f;
        position: relative;
    }

    .roadLine{
        width: 100%;
        border-top-style: dashed;
        border-top-width: 15px;
        border-top-color: #fff;

        /*background-image: linear-gradient(90deg, transparent, transparent 50%, #636b6f 50%, #636b6f 70%), linear-gradient(90deg, #fff, #fff );*/
        /*background-size: 150px 30px, 100% 3px;*/
        position: absolute;
        top: 42%;
        background-repeat: repeat-x;
        /*animation: roadLine 4s linear infinite;*/
    }
@keyframes roadLine {
    0% {
        transform: translate(0, 0)
    }
    100% {
        transform: translate(100%, 0);
    }
    /*100% {*/
    /*    transform: translate(100%, 0);*/
    /*}*/
}
    .car{
        position: absolute;
        background: url("../assets/picture/gruzovik.png") no-repeat center center;
        background-size: cover;
        height: 80px ;
        width: 140px;
        right: 10px;
        animation: car-drive 1s linear infinite alternate;
    }
@keyframes car-drive {
    0% {
        transform: translate(0, 0)
    }
    100% {
        transform: translate(0, 10px);
    }
}
@media screen and (max-width: 425px) {
    .containerHeader{
        max-width: 300px;
    }
    #gryz{
        font-size: 32px;
        margin-right: 5px;
    }
    #bel{
        font-size: 25px;
        margin: 0px 5px;
    }

}

    /*@keyframes background {*/
    /*0% {*/
    /*    transform: translate(0, 0);*/
    /*    opacity: 10%;*/
    /*}*/
    /*10%{*/
    /*    transform: translate(-10%, 0);*/
    /*    opacity: 100%;*/
    /*}*/
    /*98% {*/
    /*    transform: translate(-460%, 0);*/
    /*    opacity: 100%;*/
    /*}*/
    /*100% {*/
    /*    transform: translate(-480%, 0);*/
    /*    opacity: 0%;*/
    /*}*/

</style>
