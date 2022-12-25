<template>
  <div class="wrapper">
    <navigationTop />
    <transferContinue />
    <socialIcons />
    <leadingPlatform />
    <changeSteps />
    <countriesApp />

    <div class="FaqAnswers__wrapper faqanswers _container">
      <div class="FaqAnswers__text">
        <h1 class="_header-sections">FAQ</h1>
        <p>Найдите ответы на интересующие вопросы</p>
      </div>
      <div class="faqanswers__items">
        <div v-for="item in list" :key="item.id">
          <FaqAnswers v-bind:article="item" />
        </div>
      </div>
    </div>

    <changeMoneyFast />
    <footerSocial />
  </div>
</template>

<script>
import navigationTop from "./components/navigationTop.vue";
import transferContinue from "./components/transfer.vue";
import leadingPlatform from "./components/leadingPlatform.vue";
import changeSteps from "./components/changeSteps.vue";
import countriesApp from "./components/countriesApp.vue";
import FaqAnswers from "./components/FaqAnswers.vue";
import changeMoneyFast from "./components/changeMoneyFast.vue";
import footerSocial from "./components/footerSocial.vue";
import socialIcons from "./components/SocialIcons.vue";
export default {
  name: "App",
  components: {
    navigationTop,
    transferContinue,
    socialIcons,
    leadingPlatform,
    changeSteps,
    countriesApp,
    FaqAnswers,
    changeMoneyFast,
    footerSocial,
  },
  data() {
    return {
      list: [],
      item: {},
    };
  },
  async mounted() {
    const result = await fetch("list.json");
    const data = await result.json();
    this.list = data;
  },
};
</script>

<style>
@import url("../src/normalize.css");
@font-face {
  font-family: "TT Firs Neue";
  src: url("./fonts/TTFirsNeue/TTFirsNeue-Medium.eot");
  src: local("./fonts/TTFirsNeue/TT Firs Neue Medium"), local("TTFirsNeue-Medium"),
    url("./fonts/TTFirsNeue/TTFirsNeue-Medium.eot?#iefix") format("embedded-opentype"),
    url("./fonts/TTFirsNeue/TTFirsNeue-Medium.woff2") format("woff2"),
    url("./fonts/TTFirsNeue/TTFirsNeue-Medium.woff") format("woff"),
    url("./fonts/TTFirsNeue/TTFirsNeue-Medium.ttf") format("truetype");
  font-weight: 500;
  font-style: normal;
}
body {
  font-family: "TT Firs Neue";
}
[class*="_container"] {
  max-width: 1254px;
  margin: 0 auto;
  padding: 0 15px;
}
.wrapper {
  min-height: 100%;
  display: flex;
  flex-direction: column;
  overflow: clip;
}
._header-sections {
  font-style: normal;
  font-weight: 500;
  font-size: 48px;
  line-height: 117%;
  color: #000000;
}
@media (max-width: 400px) {
  ._header-sections {
    margin-bottom: 20px;
    font-size: 32px;
  }
}
.button-blue {
  flex: 0 1 auto;
  display: flex;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #ffffff;
  padding: 12px 16px;
  background: #3e8bf3;
  border-radius: 8px;
  align-items: center;
  justify-content: center;
  min-width: 141px;
}
.button-blue:hover {
  background: #3474ca;
}
.button-blue:active {
  background: #295da2;
}
/* transitions */
.transition-content-enter-active,
.transition-content-leave-active {
  transition: all 0.5s ease;
}
.transition-content-enter-from,
.transition-content-leave-to {
  opacity: 0;
  transform: translateX(200px);
}
/*end transitions */
</style>
