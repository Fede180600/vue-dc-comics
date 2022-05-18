<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader />
    <!-- MAIN -->
    <main>
      <AppBanner />
      <div class="container">
        <AppSeriesList />
      </div>
    </main>
    <AppBlueLine />
    <!-- FOOTER -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppBanner from "./components/AppBanner.vue"
import AppSeriesList from "./components/AppSeriesList.vue";
import AppBlueLine from "./components/AppBlueLine.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppBanner,
    AppSeriesList,
    AppBlueLine,
    AppFooter,
  },
};
</script>

<style>
@import "./style/common.scss";
main {
  width: 100%;
  color: white;
  background-color: #1c1c1c;
}
</style>
