<script>
import appHeader from "./components/appHeader.vue";
import appMain from "./components/appMain.vue";
import banner from "./components/banner.vue";

export default {
  components: {
    appHeader,
    appMain,
    banner,    
  },
};
</script>

<template>
  
  <appHeader />
  <appMain />
  <banner />

  
 
  
</template>

<style lang="scss">
@use "./style/general.scss";
</style>