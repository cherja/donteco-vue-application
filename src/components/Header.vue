<template>
  <div class="header-container">
    <div class="header-content">
      <div class="header_logo">
        <img src=../assets/images/header__logo.png>
      </div>
      <div class="header_img">
        <transition name="bounce">
          <div class="img-animation"/>
        </transition>
      </div>
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
  width: 1800px;
  margin: auto;
}

.header-content {
  display: flex;
  justify-content: space-between;
  margin-right: 50px;
}

.header_logo>img {
  width: 100%;
}

.header_img {
  width: 800px;
  height: 400px;
  overflow: hidden;
  position: relative;
}

.img-animation {
  background-image: url(../assets/images/companystaff.png);
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
    transform: scale(1.1);
  }
}

.header__front__contacts {
  color: #11449d;
  align-self: flex-end;
  a {
    color: #11449d;
    font-weight: 900;
    text-decoration: none;
  }
}

.header__background__bottomText {
  position: relative;
}

.header__background__bottomText>p {
  top: 17%;
  left: -37%;
  position: absolute;
  color: #11449d;
  font-size: 2.2em;
  line-height: 38px;
}

.header__background__bottomText>img {
  width: 260px;
}

</style>
