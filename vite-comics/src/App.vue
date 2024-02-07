<script>
import HeaderApp from "./components/HeaderApp.vue";
import JumbotronApp from "./components/JumbotronApp.vue";
import FooterApp from "./components/FooterApp.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    HeaderApp,
    JumbotronApp,
    FooterApp,
    Footer
  }
};
</script>

<template>
  <HeaderApp/>
  <JumbotronApp/>
  <FooterApp/>
  <Footer/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
