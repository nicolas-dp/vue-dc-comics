<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <SiteBanner />
    <SiteFooterCenter />
    
    <footer class="footer_end_menu">
      <div class="container">
        <div class="payment">
          <div class="button">
            <a>sing-up now</a>
          </div>

          <div class="follow">
            <span>
              <h4>FOLLOW US</h4>
            </span>
            <a href="#"
              ><img src="@/assets/img/footer-facebook.png" alt=""
            /></a>
            <a href="#"
              ><img src="@/assets/img/footer-facebook.png" alt=""
            /></a>
            <a href="#"
              ><img src="@/assets/img/footer-facebook.png" alt=""
            /></a>
            <a href="#"
              ><img src="@/assets/img/footer-facebook.png" alt=""
            /></a>
            <a href="#"
              ><img src="@/assets/img/footer-facebook.png" alt=""
            /></a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import SiteHeader from "./components/HeaderComponent.vue";
import SiteMain from "./components/MainComponent.vue";
import SiteBanner from "./components/BannerComponent.vue";
import SiteFooterCenter from "./components/FooterCenter.vue";
export default {
  name: "App",
  components: {
    SiteHeader,
    SiteMain,
    SiteBanner,
    SiteFooterCenter,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/style.scss";


/* Footer end + menu payment*/
.footer_end_menu{
  background-color: #303030;
  height: 100%;
}

.payment {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
</style>
