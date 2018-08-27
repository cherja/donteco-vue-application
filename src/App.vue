<template>
  <div id="app" class="wrapper">
    <modalcontent
      v-if="isShow"
      @close="isShow = false"
    />
    <headercomponent @open="isShow = true"/>
    <uralauto/>
    <smartyard/>
    <gobambino/>
    <bomb/>
    <aboutcompany/>
    <companystaff/>
    <forminlayout/>
    <companyaddress/>
    <footerblock/>
  </div>
</template>

<script>
import headercomponent from './components/Header.vue'
import uralauto from './components/UralAuto.vue'
import smartyard from './components/SmartYard.vue'
import gobambino from './components/Gobambino.vue'
import bomb from './components/Bomb.vue'
import aboutcompany from './components/AboutCompany.vue'
import companystaff from './components/CompanyStaff.vue'
import forminlayout from './components/FormInLayout.vue'
import companyaddress from './components/CompanyAddress.vue'
import footerblock from './components/Footer.vue'
import modalcontent from './components/Modal.vue'

export default {
  components: {
    headercomponent,
    uralauto,
    smartyard,
    gobambino,
    bomb,
    aboutcompany,
    companystaff,
    forminlayout,
    companyaddress,
    footerblock,
    modalcontent
  },
  name: 'app',
  data () {
    return {
      isShow: false
    }
  }
}
</script>

<style lang="scss">
@import "./helpers";

@font-face {
  font-family: "BBB";
  src: url("./assets/fonts/bebasbeuebold.otf");
}

@font-face {
  font-family: "SSP";
  src: url("./assets/fonts/sourcesanspro.ttf");
}

@font-face {
  font-family: "BNB";
  src: url("./assets/fonts/bebasneuebook.ttf");
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.wrapper {
  max-width: 2000px;
  margin: auto;
  overflow: hidden;
}

.container {
  padding: 0 50px 0 320px;

   @include screen-max(1600px) {
      padding: 0 50px 0 200px;
    }

   @include screen-max(1400px) {
      padding: 0 50px 0 100px;
    }

    @include screen-md {
     padding: 0 0 0 50px;
    }

    @include screen-xs {
    padding: 0px;
  }
}
</style>
