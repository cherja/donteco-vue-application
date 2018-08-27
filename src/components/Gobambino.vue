<template>
  <div class="gobabino-block container">
    <div class="gobabino-block__text">
      <h2>Gobambino.com</h2>
      <h3>Маркет-плейс</h3>
      <p>Коммерчески успешный маркет-плейс для рынка США, состоящий из web-сервиса и мобильного приложения для iOS. Самой сложной задачей было создание максимально удобной панели администратора детских центров для ведения графика занятий и учета числа мест</p>
    </div>
    <div class="gobabino-block__img"/>
  </div>
</template>

<style lang="scss">
@import "../helpers";

.gobabino-block {
  background: linear-gradient(to right, #ec368d, #f6719a);
  display: flex;
  justify-content: space-between;
  align-items: center;
  border: 1px solid #ec368d;
   @include screen-xs {
    display: block;
  }
}

.gobabino-block__text{
  h2 {
    color: #ffffff;
    font-family: "BBB";
    font-weight: 900;
    font-size: 78px;
    @include screen-max(1850px) {
      font-size: 62px;
    }

    @include screen-max(1400px) {
      font-size: 50px;
    }

    @include screen-lg {
      font-size: 48px;
    }
  }

  h3 {
    color: #ffffff;
    font-family: "SSP";
    font-size: 43px;
    font-weight: 100;
    line-height:1.1;
     @include screen-max(1850px) {
      font-size: 35px;
    }

    @include screen-max(1400px) {
      font-size: 31px;
    }

    @include screen-lg {
      font-size: 28px;
    }

  }

  p {
    color: #ffffff;
    margin-top: 80px;
    font-size: 23px;
    font-weight: 100;
    line-height:1.6;
    width: 450px;
     @include screen-max(1850px) {
      font-size: 19px;
    }
    @include screen-max(1400px) {
      font-size: 17px;
      margin-top: 60px;
    }
    @include screen-lg {
      font-size: 16px;
      margin-top: 40px;
    }

    @include screen-sm {
      margin-top: 30px;
      width: 320px;
    }
  }
      @include screen-xs {
      margin: 50px auto;
      width: 320px;
    }
}

.gobabino-block__img {
  width: 806px;
  height: 632px;
  background-position: center center;
  background-size: contain;
  background-repeat: no-repeat;
  background-image: url(../assets/images/imac.png);
  margin: 100px 0 100px 30px;
  @include screen-max(1400px) {
      width: 604px;
      height: 474px;
    }
     @include screen-lg {
      width: 483px;
      height: 379px;
    }
    @include screen-md {
      width: 483px;
      height: 379px;
      background-size: cover;
     background-position: left center;
    }
      @include screen-xs {
      width: 320px;
      height: 300px;
      background-size: contain;
      margin:auto;
     margin: 50px auto;
    }
    @include screen-max(450px) {
      width: 300px;
      height: 300px;
    }
  }

</style>
