<template>
  <menuAside v-bind:list="list" />
  <navigationTop />
  <launchApp />
  <transferContinue />
  <leadingPlatform />
  <changeSteps />
  <countriesApp />
  <faqAnswers />
  <changeMoneyFast />
  <footerSocial />
</template>

<script>
/*import menuAside from "./components/menuAside.vue";*/
import navigationTop from "./components/navigation.vue";
import launchApp from "./components/launchApp.vue";
import transferContinue from "./components/transfer.vue";
import leadingPlatform from "./components/leadingPlatform.vue";
import changeSteps from "./components/changeSteps.vue";
import countriesApp from "./components/countriesApp.vue";
import faqAnswers from "./components/faqAnswers.vue";
import changeMoneyFast from "./components/changeMoneyFast.vue";
import footerSocial from "./components/footerSocial.vue";
export default {
  name: "App",
  components: {
    /*menuAside, */
    navigationTop,
    launchApp,
    transferContinue,
    leadingPlatform,
    changeSteps,
    countriesApp,
    faqAnswers,
    changeMoneyFast,
    footerSocial,
  },
  /* props: ["list"],*/
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
