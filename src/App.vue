<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader />
    <!-- MAIN -->
    <main>
      <div class="container">
        Content goes here
      </div>
    </main>
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
@import "./style/common.scss";
main {
  width: 100%;
  padding: 50px 0;
  color: white;
  background-color: #1c1c1c;
}
</style>
