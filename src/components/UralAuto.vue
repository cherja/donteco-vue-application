<template>
  <div class="ural-auto-block container">
    <div class="ural-auto-block__text">
      <h2>URAL AUTO</h2>
      <h3>Мобильный магазин</h3>
      <p>Разработка мобильного магазина в виде мобильного приложения для iOS и Android для крупнейшего производителя автомобильной акустики в России</p>
    </div>
    <div class="ural-auto-block__img">
      <div class="ural-auto-block__img-mobile ural-auto-block__img-ural-one"></div>
      <div class="ural-auto-block__img-mobile ural-auto-block__img-ural-two"></div>
    </div>
  </div>
</template>

<style lang="scss">
@import "../helpers";

.ural-auto-block.container {
  padding-top: 100px;
  padding-bottom: 100px;
  @include screen-md {
    padding-top: 50px;
    padding-bottom: 50px;
  }
}

.ural-auto-block {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #e31e3a;

  @include screen-md {
    justify-content: flex-start;
  }
   @include screen-xs {
    display: block;
  }
  h2 {
    font-family: "BBB";
    font-weight: 900;
    font-size: 78px;
    color: #ffffff;
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
    font-family: "SSP";
    margin-top: 80px;
    font-size: 23px;
    font-weight: 100;
    line-height:1.6;
    width: 390px;
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
      width: auto;
    }
  }
}

.ural-auto-block__text {
  @include screen-xs {
    width: 320px;
    margin: auto;
  }
}

.ural-auto-block__img {
  display: flex;
  margin-left: 20px;
  @include screen-xs {
    margin-top: 20px;
    justify-content: center;
  }
}

.ural-auto-block__img-mobile {
  width: 255px;
  height: 521px;
  background-position: center center;
  background-size: contain;
  background-repeat: no-repeat;
   @include screen-lg {
      width: 181px;
      height: 380px;
    }

    @include screen-md {
       width: 131px;
       height: 280px;
     }

     @include screen-sm{
       width: 100px;
       height: 230px;
     }
  @include screen-xs {
    width: 181px;
    height: 210px;
  }
}

.ural-auto-block__img-ural-one {
    background-image: url(../assets/images/ural_smart_one.png);
      @include screen-sm {
      margin-right: 20px;
    }
}

.ural-auto-block__img-ural-two {
  margin: 50px 50px 0 50px;
    background-image: url(../assets/images/ural_smart_two.png);

     @include screen-md {
       margin: 50px 10px 0 20px;
     }

     @include screen-xs {
       display: flex;
       margin: 30px 10px 0 20px;
     }
}
</style>
