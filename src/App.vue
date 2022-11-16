<template>
  <navigationTop />
  <launchApp />
  <transferContinue />
  <leadingPlatform />
  <changeSteps />
  <countriesApp />
  <FaqAnswers v-bind:list="list" />
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
    };
  },
  async mounted() {
    const result = await fetch("./assets/list.json");
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
</style>
