<template>
  <div class="container">
    <Header></Header>
    <div class="line-under-blok"></div>
    <DivPrice></DivPrice>
    <div class="line-under-blok"></div>
    <DivTransp></DivTransp>
    <div class="line-under-blok"></div>
    <DivServices></DivServices>
    <div class="line-under-blok"></div>
    <DivOppSale></DivOppSale>
    <br>
    <div class="line-under-blok"></div>
    <TypePayment></TypePayment>
    <div class="line-under-blok"></div>
    <Contacts></Contacts>

  </div>
</template>

<script>
  import Header from './components/Header'
  import DivTransp from './components/DivTransp'
  import DivPrice from './components/DivPrice'
  import DivServices from './components/DivServices'
  import DivOppSale from './components/DivOppSale'
  import Contacts from './components/Contacts'
  import TypePayment from './components/typePayment'

  export default {
    name: 'App',
    components: { TypePayment, Contacts, DivOppSale, DivServices, DivTransp, Header, DivPrice }
  }
</script>

<style scoped>
  i{
    font-size: 25px;
  }
  .container{

    width: 100%;
    max-width: 800px;
    min-height: 100vh;
    /*background-color: #6cb2eb;*/
    margin: 0 auto;

  }
  @media screen and (max-width: 376px) {
    .container{
      margin: 0;
    }
  }

  .line-under-blok{
    height: 5px;
    background-color: black;
  }

</style>
