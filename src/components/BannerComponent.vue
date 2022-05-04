<template>
  <div class="site_footer">
    <div class="container">
      <div class="footer_menu" >
        <a href="#" v-for="item in banner" :key="item.id">
          <img :src="item.src" :alt="item.text" />
          <span>{{ item.text }}</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SiteBanner",
  data() {
    return {
      banner: [
        {
          id: 1,
          src: require("@/assets/img/buy-comics-digital-comics.png"),
          text: "digital comics",
        },
        {
          id: 2,
          src: require("@/assets/img/buy-comics-merchandise.png"),
          text: "dc merchandise",
        },
        {
          id: 3,
          src: require("@/assets/img/buy-comics-subscriptions.png"),
          text: "subscription",
        },
        {
          id: 4,
          src: require("@/assets/img/buy-comics-shop-locator.png"),
          text: "comic shop locator",
        },
        {
          id: 5,
          src: require("@/assets/img/buy-dc-power-visa.svg"),
          text: "dc power visa",
        }
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

.site_footer {
  background-color: $dc-primary;
}

.footer_menu {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding: 1rem;

  &>a {
    color: $dc-white;
    display: flex;
    border: none;
    align-items: center;
    flex-wrap: wrap;
    padding: 1rem;
    font-size: 14px;
  }

  img{
      height: 50px;
  } 
}
</style>