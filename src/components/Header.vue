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
      <div class="razriv"></div>
      <div class="header_img">
        <transition name="bounce">
          <div class="img-animation"/>
        </transition>
      </div>
    </div>
    <div class="header-content colu">
      <div @click="$emit('open')" class=header__front__call>
        <p>Заказать звонок</p>
      </div>
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
.colu {
  @include screen-max(1100px) {
  flex-direction: column-reverse;
  }
}

.header__front__call {
  display: none;
}

.header__front__call {
  @include screen-max(1100px) {
    width: 31%;
    background: #11449d;
    height: 48px;
    border-radius: 3px;
    display: flex;
    @include screen-max(880px) {
      width: 51%;
    }
  }
}
.header__front__call>p {
  display:flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  color: white;
  font-size: 2.8vw;
  margin: 0;
  @include screen-max(880px) {
      font-size: 4.8vw;
    }
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
   @include screen-max(1220px) {
    top: 50%;
  }
  @include screen-max(880px) {
    top: 65%;
  }
    @include screen-max(880px) {
      font-size: 60px;
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
    @include screen-max(880px) {
      height: 75px;
    }
    @include screen-max(410px) {
      height: 70px;
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
  @include screen-max(410px) {
      font-size: 60px
    }
}

.header__front__bigText__1 {
  width: 32%;
  @include screen-max(960px) {
      width:350px;
    }
    @include screen-max(410px) {
      width:300px;
    }
}

.header__front__bigText__2 {
     width: 30%;
     @include screen-max(960px) {
      width:320px;
    }
    @include screen-max(410px) {
      width:290px;
    }
}

.header__front__bigText__3 {
  width: 33%;
  @include screen-max(960px) {
      width:350px;
    }
    @include screen-max(410px) {
      width:310px;
    }
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

.razriv {
   @include screen-max(1100px) {
    width:100%;
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
  @include screen-max(410px) {
    padding: 0 0 0 10px;
  }
}

.header_logo {
  width: 20%;
  margin-top: 40px;
  @include screen-max(880px) {
    width: 30%;
  }
  @include screen-max(880px) {
    width: 40%;
  }
  @include screen-max(410px) {
    width: 50%;
  }
}

.header_logo>img {
  width: 100%;
}

.header_img {
  width: 75%;
  height: 670px;
  overflow: hidden;
  position: relative;
  @include screen-max(1720px) {
    height: 520px;
  }

   @include screen-max(1400px) {
    height: 450px;
  }
  @include screen-max(1100px) {
    margin: 30px 0 80px 20px;
    width: 100%;
  }
  @include screen-max(880px) {
    margin: 30px 0 180px 20px;
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
  @include screen-max(1100px) {
    align-self: auto;
  }
  @include screen-max(1100px) {
    margin: 40px 0;
  }
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
    @include screen-max(1100px) {
     font-size: 23px;
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
   @include screen-max(1100px) {
    font-size: 31px;
    left: 0px;
    top: 15%;
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
  @include screen-max(1110px) {
    margin-left: 90px;
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
