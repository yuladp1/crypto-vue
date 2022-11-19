<template>
  <navigationTop />
  <launchApp />
  <transferContinue />
  <leadingPlatform />
  <changeSteps />
  <countriesApp />
  <h1>FAQ</h1>
  <p>Найдите ответы, на интересующие вопросы</p>
  <div v-for="item in list" :key="item.id">
    <FaqAnswers v-bind:article="item" />
  </div>

  <changeMoneyFast />
  <footerSocial />
</template>

<script>
import navigationTop from "./components/navigation.vue";
import launchApp from "./components/launchApp.vue";
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
    launchApp,
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
    console.log(this.list);
  },
};
</script>

<style>
body {
  margin: 0;
}
figure {
  margin-block-start: 0;
  margin-block-end: 0;
  margin-inline-start: 0;
  margin-inline-end: 0;
}
p {
  font-size: 14px;
  font-weight: 500;
  line-height: 20px;
  text-align: left;
  color: #6f767e;
}
</style>
