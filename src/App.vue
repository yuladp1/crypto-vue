<template>
  <menuAside />
  <navigationTop />
  <launchApp />
  <transferContinue />
  <leadingPlatform />
  <changeSteps />
  <countriesApp />
  <faqAnswers />
</template>

<script>
import menuAside from "./components/menuAside.vue";
import navigationTop from "./components/navigation.vue";
import launchApp from "./components/launchApp.vue";
import transferContinue from "./components/transfer.vue";
import leadingPlatform from "./components/leadingPlatform.vue";
import changeSteps from "./components/changeSteps.vue";
import countriesApp from "./components/countriesApp.vue";
import faqAnswers from "./components/faqAnswers.vue";
export default {
  name: "App",
  components: {
    menuAside,
    navigationTop,
    launchApp,
    transferContinue,
    leadingPlatform,
    changeSteps,
    countriesApp,
    faqAnswers,
  },
};
</script>

<style>
body {
  margin: 0;
}
</style>
