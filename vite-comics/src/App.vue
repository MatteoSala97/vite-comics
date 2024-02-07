<script>
import HeaderApp from "./components/HeaderApp.vue";
import JumbotronApp from "./components/JumbotronApp.vue";

export default {
  components: {
    HeaderApp,
    JumbotronApp,
  }
};
</script>

<template>
  <HeaderApp/>
  <JumbotronApp/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
