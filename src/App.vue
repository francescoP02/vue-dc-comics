<template>
  <div id="app">
    <header>
      <AppHeader />
    </header>

    <main>
      <ComicList />
      <AppShop />
    </main>

    <footer>
      <AppFooter />
    </footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import ComicList from "./components/ComicList.vue";
import AppShop from "./components/AppShop.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    ComicList,
    AppShop,
    AppFooter,
  },
};
</script>

<style lang="scss"></style>
