<template>
  <div class="footer-block container">
    <div class="footer-block-content">
      <div class="footer-block-logo">
        <div class="footer-block-logo__img"/>
        <p>Donteco</p>
      </div>
      <div class="footer-block-contacts">
       <p>Москва  <a href="tel: +74953746795">8(495)374-67-95</a></p>
       <p>Ростов-на-Дону  <a href="tel: +78633200167">8(863)320-01-67</a></p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import "../helpers";

.footer-block {
  width: 100%;
  background-color: #0a3278;
  color: #ffffff;
  &-logo {
    display: flex;
    align-items: center;
    font-size: 23px;
    font-family: "SSP";
    font-weight: 600;
  }
  .footer-block-logo__img {
    margin: 0 5px 0 10px;
    width: 28px;
    height: 28px;
    background-position: center center;
    background-size: contain;
    background-repeat: no-repeat;
    background-image: url(../assets/images/logo.png);
  }
}

.footer-block-contacts {
  display: flex;
    a {
    color: #ffffff;
    font-family: "SSP";
    text-decoration: none;
    margin: 0 7px;
    }
  p {
    font-family: "SSP";
    margin: 0 25px;
  }
  @include screen-sm {
     display: block;
  }
  @include screen-max(450px) {
    margin-top:30px;
  }
}

.footer-block-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 30px 0 50px 0;
  @include screen-sm {
     padding: 20px 0 30px 0;
  }
  @include screen-max(450px) {
      flex-direction: column;
      align-items: flex-start;
    }
}

</style>
