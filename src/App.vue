<script>
import appHeader from "./components/appHeader.vue";
import appMain from "./components/appMain.vue";
import banner from "./components/banner.vue";
import footerTop from "./components/footerTop.vue"

export default {
  components: {
    appHeader,
    appMain,
    banner, 
    footerTop   
  },
};
</script>

<template>
  
  <appHeader />
  <appMain />
  <banner />
  <footerTop />

  
 
  
</template>

<style lang="scss">
@use "./style/general.scss";
</style>