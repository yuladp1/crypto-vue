<template>
  <div class="wrapper">
    <navigationTop />
    <transferContinue />
    <leadingPlatform />
    <changeSteps />
    <countriesApp />

    <div class="wrapper-FaqAnswers-large">
      <div class="wrapper-FaqAnswers">
        <h1 id="faq">FAQ</h1>
        <p>Найдите ответы на интересующие вопросы</p>
      </div>
      <div class="wrapper-items-large">
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
export default {
  name: "App",
  components: {
    navigationTop,
    transferContinue,
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
  src: url("./fonts/TTFirsNeue/TTFirsNeue-Light.woff");
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
</style>
