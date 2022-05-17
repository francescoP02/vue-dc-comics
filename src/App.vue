<template>
  <div id="app">
    <AppHeader />
    <AppContent />
    <AppShop />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppContent from "./components/AppContent.vue";
import AppShop from "./components/AppShop.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppContent,
    AppShop,
    AppFooter,
  },
};
</script>

<style lang="scss"></style>
