<template>
  <div class="bomb-block container">
    <div class="bomb-block__text">
      <h2>BOMB RIDERS</h2>
      <h3>Мобильная игра</h3>
      <p>Угарная игрушка для мобильных телефонов и планшетов, сделанная по мотивам старых игр серии Bomberman, но с потрясающей графикой от нашего штатного дизайнера-иллюстратора. Решение включает разработку на Unity 3D, создание сервера мультиплеерной игры и написание человекоподобного искусственного интеллекта противников</p>
    </div>
    <div class="bomb-block__img">
      <div class="bomb-block__img-mobile bomb-block__img-smart-one"></div>
      <div class="bomb-block__img-mobile bomb-block__img-smart-two"></div>
    </div>
  </div>
</template>

<style lang="scss">
@import "../helpers";

.bomb-block {
  display: flex;
    justify-content: space-between;
  align-items: flex-end;
   @include screen-max(1850px) {
      align-items: center;
    }
    @include screen-xs {
    display: block;
  }
}
.bomb-block.container {
  padding-bottom: 50px;
  padding-top: 50px;
}

.bomb-block__text {
   width: 500px;
   margin-right: 30px;
   @include screen-max(1400px) {
      width: 400px;
    }
       @include screen-md {
      width: 350px;
    }

     @include screen-sm {
       width: 500px;
    }
    @include screen-xs {
    width: 320px;
        margin: auto;
  }
  h2 {
    font-family: "BBB";
    font-weight: 900;
    font-size: 78px;
    color: #5bcf03;
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
    font-family: "SSP";
    margin-top: 80px;
    font-size: 23px;
    font-weight: 100;
    line-height:1.6;
     @include screen-max(1850px) {
      font-size: 20px;
    }
    @include screen-max(1400px) {
      font-size: 18px;
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
}

.bomb-block__img {
   @include screen-md {
      overflow:hidden;
    }
}

.bomb-block__img-mobile {
  width: 605px;
  height: 305px;
  background-position: center center;
  background-size: contain;
  background-repeat: no-repeat;
  @include screen-max(1400px) {
    width: 484px;
    height: 244px;
  }
  @include screen-md {
        width: 387px;
    height: 195px;
    }
     @include screen-sm {
         width: 309px;
    height: 156px;
    }
     @include screen-xs {
      margin: auto;
    }
}

.bomb-block__img-smart-one {
  background-image: url(../assets/images/smartbombone.png);
  margin-top: 100px;
  margin-left: 200px;
  @include screen-max(1550px) {
      margin-left: 100px;
    }

    @include screen-lg {
      margin-left: 50px;
    }
    @include screen-xs {
      margin: 50px auto 0 auto;
    }
}

.bomb-block__img-smart-two {
  background-image: url(../assets/images/smartbombtwo.png);
}
</style>
