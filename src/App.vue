<script>
import appHeader from "./components/appHeader.vue";
import appJumbotron from "./components/appJumbotron.vue";
import appMain from "./components/appMain.vue";
import appBanner from "./components/appBanner.vue";
import appFooterTop from "./components/appFooterTop.vue";
import appFooterBottom from "./components/appFooterBottom.vue";

export default {
  components: {
    appHeader,
    appMain,
    appJumbotron,
    appBanner, 
    appFooterTop,
    appFooterBottom  
  },
};
</script>

<template>
  
  <appHeader />
  <appMain />
  <appJumbotron />
  <appBanner />
  <appFooterTop />
  <appFooterBottom />

  
 
  
</template>

<style lang="scss">
@use "./style/general.scss";
</style>