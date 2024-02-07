<script>
import HeaderApp from "./components/HeaderApp.vue";
import JumbotronApp from "./components/JumbotronApp.vue";
import FooterApp from "./components/FooterApp.vue";

export default {
  components: {
    HeaderApp,
    JumbotronApp,
    FooterApp,
  }
};
</script>

<template>
  <HeaderApp/>
  <JumbotronApp/>
  <FooterApp/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
