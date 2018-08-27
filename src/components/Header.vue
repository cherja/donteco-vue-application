<template>
  <div class="header-container">
    <div class="header-content">
      <div class=header__front__bigText>
        <div class=header__front__bigText__1><p>РАЗРАБОТКА</p></div>
        <div class=header__front__bigText__2><p>МОБИЛЬНЫХ</p></div>
        <div class=header__front__bigText__3><p>ПРИЛОЖЕНИЙ</p></div>
      </div>
      <div class="header_logo">
        <img src=../assets/images/header__logo.png>
      </div>
      <div class="line-break"></div>
      <div class="header_img">
        <div @click="$emit('open')" class=header__front__call__hd>
          <p>ЗАКАЗАТЬ ЗВОНОК</p>
          <p class="line"></p>
        </div>
        <transition name="bounce">
          <div class="img-animation"/>
        </transition>
      </div>
    </div>
    <div @click="$emit('open')" class=header__front__call>
      <p>Заказать звонок</p>
    </div>
    <div class="header-content">
      <div class="header__front__contacts">
        <p>Москва <a href="tel: +74953746795">8(495)374-67-95</a></p>
        <p>Ростов-на-Дону <a href="tel: +78633200167">8(863)320-01-67</a></p>
      </div>
      <div class=header__background__bottomText>
        <img src=../assets/images/header__100.png>
        <p>Более<br>реализованных<br>проектов!</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import "../helpers";
.header__front__call {
  display: none;
}

.header__front__call {
  @include screen-max(1100px) {
    width: 31%;
    background: #11449d;
    height: 38px;
    position: absolute;
    border-radius: 3px;
    bottom: 100px;
    left: 0;
    display: flex;
    align-items: center;
  }
}
.header__front__call>p {
  text-align: center;
  width: 100%;
  color: white;
  font-size: 2.8vw;
  margin: 0;
}

.header__front__bigText {
  position: absolute;
  top: 174px;
  z-index: 3;
   @include screen-max(1720px) {
    top: 124px;
  }
}

.header__front__bigText>div {
  background: #25ced1;
  height: 115px;
  margin: 24.48px 0 0;
   @include screen-max(1720px) {
    height: 100px;
  }
}

.header__front__bigText>div>p {
  font-weight: 500;
  font-family: "BNB";
  font-size: 115px;
  letter-spacing: 5px;
  color: white;
  position: relative;
  top: -8px;
  left: 8px;
   @include screen-max(1720px) {
    font-size: 95px;
    top: 8px;
  }
}

.header__front__bigText__1 {
  width: 530px;
   @include screen-max(1720px) {
    width: 440px;
  }
}

.header__front__bigText__2 {
  width: 505px;
   @include screen-max(1720px) {
    width: 410px;
  }
}

.header__front__bigText__3 {
  width: 560px;
   @include screen-max(1720px) {
    width: 470px;
  }
}

.header__front__call__hd {
  z-index: 2;
  display: flex;
  align-items: center;
  position: absolute;
  right: -28%;
  bottom: 460px;
  transform: rotate(-90deg);
  font-size: 27px;
  color: #11449d;
  cursor: pointer;
  @include screen-max(1720px) {
    right: -36%;
    bottom: 420px;
  }
  @include screen-max(1720px) {
    right: -47%;
    bottom: 425px;
  }
}

.line {
 width: 600px;
 border: 1px solid #11449d;
}

.header-content {
  font-family: "SSP";
  max-width: 1680px;
  margin: auto;
  padding: 0 50px;
  display: flex;
  justify-content: space-between;
  margin-right: 50px;
  flex-wrap: wrap;
  position: relative;
}
.header-content:last-child {
  margin-bottom: 50px;
}
// .line-break {
//   width: 100%;
// }

.header_logo>img {
  width: 100%;
   @include screen-max(1450px) {
    width: 80%;
  }
}

.header_logo {
  position: absolute;
  top: 40px;
}

.header_img {
  width: 1400px;
  height: 770px;
  overflow: hidden;
  position: relative;
   @include screen-max(1720px) {
    width: 1100px;
    height: 550px;
  }
  @include screen-max(1450px) {
    width: 850px;
    height: 450px;
  }
}

.img-animation {
  background-image: url(../assets/images/header_main.png);
  position: absolute;
  animation: bounce-in 4s linear forwards;
  background-position: center center;
  background-size: cover;
  top:0;
  left:0;
  right:0;
  bottom: 0;
}

@keyframes bounce-in {
  0% {
    transform: scale(1);
  }

   70% {
    transform: scale(1.08);
  }

  100% {
    transform: scale(1.09);
  }
}

.header__front__contacts {
  color: #11449d;
  align-self: flex-end;
  p, a {
    font-size: 23px;
     @include screen-max(1850px) {
      font-size: 19px;
    }
    @include screen-max(1400px) {
      font-size: 17px;
    }
    @include screen-lg {
      font-size: 16px;
    }
  }
  a {
    color: #11449d;
    font-weight: 900;
    text-decoration: none;
  }
}

.header__background__bottomText {
  position: relative;
  margin-right: 30px;
}

.header__background__bottomText>p {
  top: 37%;
  left: -37%;
  position: absolute;
  color: #11449d;
  font-size: 51px;
  line-height: 38px;
  font-weight: 900;

}

.header__background__bottomText>img {
  width: 370px;
  @include screen-max(1720px) {
    width: 300px;
  }
}

</style>
