<script>
import appHeader from "./components/appHeader.vue";
import appMain from "./components/appMain.vue";

export default {
  components: {
    appHeader,
    appMain    
  },
};
</script>

<template>
  
  <appHeader />
  <appMain />

  
 
  
</template>

<style lang="scss">
@use "./style/general.scss";
</style>