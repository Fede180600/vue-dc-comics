<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader />
    <!-- MAIN -->
    <main>Main</main>
    <AppBlueLine />
    <!-- FOOTER -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppBlueLine from "./components/AppBlueLine.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppBlueLine,
    AppFooter,
  },
};
</script>

<style>

</style>
