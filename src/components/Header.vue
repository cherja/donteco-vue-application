<template>
  <div class="header-container">
    <div class="header-content">
      <div @click="$emit('open')" class=header__front__call__hd>
        <p>ЗАКАЗАТЬ ЗВОНОК</p>
        <p class="line"></p>
      </div>
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
.header-container {
  position: relative;
}

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
    left: 50px;
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
  width: 100%;
   @include screen-max(1720px) {
    top: 110px;
  }
  @include screen-max(1220px) {
    width: 110%;
  }
}

.header__front__bigText>div {
  background: #25ced1;
  height: 115px;
  margin: 24.48px 0 0;
    @include screen-max(1720px) {
      height: 95px;
    }
    @include screen-max(1400px) {
      height: 85px;
    }
}

.header__front__bigText>div>p {
  font-weight: 500;
  font-family: "BNB";
  font-size: 115px;
  letter-spacing: 5px;
  color: white;
  position: relative;
  top: 6px;
  left: 8px;
  @include screen-max(1720px) {
    font-size: 90px;
    top: 8px;
  }
  @include screen-max(1400px) {
    font-size: 80px;
  }
  @include screen-max(1100px) {
    font-size: 70px;
  }
}

.header__front__bigText__1 {
  width: 32%;
}

.header__front__bigText__2 {
     width: 30%;
}

.header__front__bigText__3 {
  width: 33%;
}

.header__front__call__hd {
  font-weight: 900;
  z-index: 2;
  display: flex;
  align-items: center;
  position: absolute;
  transform-origin: 0px 0px;
  transform: rotate(-90deg);
  bottom: -28px;
  right:-680px;
  font-size: 27px;
  color: #11449d;
  cursor: pointer;
  @include screen-max(1100px) {
    display: none;
  }
}

.line {
 width: 500px;
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
  margin-bottom: 50px;
  flex-wrap: wrap;
  position: relative;
   @include screen-max(1100px) {
    padding: 0 0 0 50px;
    margin-right: 0px;
  }
}

.header_logo {
  width: 20%;
}

.header_logo>img {
  width: 100%;
}

.header_logo {
  position: absolute;
  top: 40px;
}

.header_img {
  width: 75%;
  height: 670px;
  overflow: hidden;
  position: relative;
  @include screen-max(1720px) {
    height: 520px;
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
   @include screen-max(1720px) {
    font-size: 41px;
    top: 20%;
    left: -40%;
  }
}

.header__background__bottomText>img {
  width: 370px;
  @include screen-max(1720px) {
    width: 280px;
  }
  @include screen-max(1720px) {
    width: 250px;
  }
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
</style>
