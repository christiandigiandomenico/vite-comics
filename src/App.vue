<script>
import AppNav from './components/AppNav.vue';
import AppContent from './components/AppContent.vue';
import AppMerchandise from './components/AppMerchandise.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppNav,
    AppContent,
    AppMerchandise,
    AppFooter
  }
}
</script>

<template>
  <AppNav></AppNav>
  <AppContent></AppContent>
  <AppMerchandise></AppMerchandise>
  <AppFooter></AppFooter>
</template>

<style></style>
