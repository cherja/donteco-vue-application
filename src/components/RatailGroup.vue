<template>
  <div class="ratail-group-block container">
    <div class="ratail-group-block__text">
      <h2>X5 Ratail Group</h2>
      <h3>Система интерактивного контента</h3>
      <p>Разработка системы управления контентом и контент-плееров для X5 Retail Group. Разработан сложный web редактор создания интерактивного контента и плееры его воспроизведения для различных платформ - прайс-чекеров, мониторов, видео-стен - для ОС Android и Windows</p>
    </div>
    <div class="ratail-group-block__img"/>
  </div>
</template>

<style lang="scss">
@import "../helpers";
.ratail-group-block.container {
   @include screen-xs {
    padding-bottom: 40px;
  }

}
.ratail-group-block {
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: white;
  background: linear-gradient(to right, #6dc2aa, #25c3ba);
  width: 100%;
  @include screen-xs {
    display: block;
  }

  h2 {
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
    color:#d2fff7;
    margin-top: 80px;
    font-size: 23px;
    font-weight: 100;
    line-height:1.6;
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
    }
  }

  &__text{
    width: 500px;
    margin-top: 80px;
    @include screen-max(1850px) {
      width: 400px;
      margin-top: 0;
      margin-right:40px;
    }

    @include screen-lg {
      width: 350px;
    }

    @include screen-sm {
      width: 600px;
    }
     @include screen-xs {
      padding: 50px 0;
      margin: auto;
      width: 310px;
    }
  }
}

.ratail-group-block__img {
  width: 895px;
  height: 632px;
  background-position: center center;
  background-size: contain;
  background-repeat: no-repeat;
  background-image: url(../assets/images/tablet.png);
  margin: 100px 0;

    @include screen-max(1850px) {
      width: 766px;
      height: 555px;
    }

    @include screen-max(1500px) {
      width: 716px;
      height: 505px;
    }

    @include screen-max(1400px) {
      width: 582px;
      height: 414px;
    }

    @include screen-lg {
      width: 465px;
      height: 331px;
    }

    @include screen-md {
    background-size: cover;
     background-position: left center;
    }
    @include screen-xs {
      margin: auto;
      width: 310px;
      height: 220px;
    }
}
</style>
