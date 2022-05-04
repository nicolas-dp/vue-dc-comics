<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <SiteBanner />
    <SiteFooterCenter />
    <SiteFooterEnd />
    
    
  </div>
</template>

<script>
import SiteHeader from "./components/HeaderComponent.vue";
import SiteMain from "./components/MainComponent.vue";
import SiteBanner from "./components/BannerComponent.vue";
import SiteFooterCenter from "./components/FooterCenter.vue";
import SiteFooterEnd from "./components/FooterEndComponent.vue";
export default {
  name: "App",
  components: {
    SiteHeader,
    SiteMain,
    SiteBanner,
    SiteFooterCenter,
    SiteFooterEnd,
  },
};
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
</style>
