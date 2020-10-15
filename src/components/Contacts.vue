<template>
    <div class="item">
        <div class="content">
            <div class="contacts">
                <div class="tel-ip">
                <i class="fa fa-phone-alt" aria-hidden="true"></i>
                <a href="tel:+375296587036"> +375 (29) 658-70-36</a>
                </div>
            </div>
            <div class="info-for-ip">
                <div><p>Индивидуальный предприниматель</p></div>
                <div class="name-ip"><p>Руденков Алексей Игоревич</p></div>

            </div>

    </div>

    </div>
</template>

<script>
export default {
  name: 'Contacts'
}
</script>

<style scoped>
    a{
        text-decoration: none;
    }
    .content{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        background-color: chocolate;
        text-align: center;
    }
    .contacts{
        text-align: center;
        font-size: 40px;
        max-width: 650px;
        border-bottom: 10px solid;
    }

    .tel-ip{
        margin: 0 auto;
    }
    .tel-ip a{
        width: auto;
        color: black;
        font-weight: bold;
    }
    .info-for-ip{
        font-size: 30px;
    }
    .name-ip{
        font-weight: bolder;
    }
    @media screen and (max-width: 375px){
        .contacts{
            font-size: 30px;
            margin: 10px;
            border-bottom: 7px solid;
        }
        .info-for-ip{
            font-size:  20px;
        }

    }

</style>
