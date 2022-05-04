<template>
  <footer class="footer_end_menu">
    <div class="container">
      <div class="payment">
        <div class="button">
          <a>sign-up now</a>
        </div>

        <div class="follow">
          <h4>FOLLOW US</h4>

          <span>
            <a href="#"
              ><img src="@/assets/img/footer-facebook.png" alt=""
            /></a>
            <a href="#"><img src="@/assets/img/footer-twitter.png" alt="" /></a>
            <a href="#"><img src="@/assets/img/footer-youtube.png" alt="" /></a>
            <a href="#"
              ><img src="@/assets/img/footer-pinterest.png" alt=""
            /></a>
            <a href="#"
              ><img src="@/assets/img/footer-periscope.png" alt=""
            /></a>
          </span>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "SiteFooterEnd",
};
</script>

<style lang="scss">
.footer_end_menu {
  background-color: $dc-dark;
  display: flex;
  flex-wrap: wrap;
  align-content: center;
  align-items: center;
  height: 15vh;
  a {
    border: none;
  }
}

.button{
    border: 1px solid $dc-primary;
    padding: 0.5rem;

    &:hover{
        filter: drop-shadow(0 0 6px white);
    }
    a{
        color: $dc-white;
    }
}

.follow {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;

  h4 {
    color: $dc-primary;
  }

  a:hover{
      filter: drop-shadow(2px 4px 6px black);
  }
}

.payment {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
</style>