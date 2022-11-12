<template>
  <navigationTop />
  <launchApp />
  <transferContinue />
</template>

<script>
import navigationTop from "./components/navigation.vue";
import launchApp from "./components/launchApp.vue";
import transferContinue from "./components/transfer.vue";
export default {
  name: "App",
  components: {
    navigationTop,
    launchApp,
    transferContinue,
  },
};
</script>

<style>
body {
  margin: 0;
}
</style>
