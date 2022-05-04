<template>
  <footer class="footer_center_menu">
    <div class="footer_bg_image">
      <div class="container">
        <div class="row">
          <div class="col-3" v-for="({title, links},index) in footerMenu" :key="index">
            <h4>{{title}}</h4>
            <ul>
              <li v-for="(link, index) in links" :key="index">{{link.text}}</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "SiteFooterCenter",
  data() {
    return {
      footerMenu: [
        {
          title: "DC COMICS",
          links: [
            {
              href: "#",
              text: "Characters",
            },
            {
              href: "#",
              text: "Comics",
            },
            {
              href: "#",
              text: "Movies",
            },
            {
              href: "#",
              text: "TV",
            },
            {
              href: "#",
              text: "Games",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "News",
            },
          ],
        },
        {
          title: "DC COMICS",
          links: [
            {
              href: "#",
              text: "Characters",
            },
            {
              href: "#",
              text: "Comics",
            },
            {
              href: "#",
              text: "Movies",
            },
            {
              href: "#",
              text: "TV",
            },
            {
              href: "#",
              text: "Games",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "News",
            },
          ],
        },
        {
          title: "DC COMICS",
          links: [
            {
              href: "#",
              text: "Characters",
            },
            {
              href: "#",
              text: "Comics",
            },
            {
              href: "#",
              text: "Movies",
            },
            {
              href: "#",
              text: "TV",
            },
            {
              href: "#",
              text: "Games",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "News",
            },
          ],
        },
        {
          title: "DC COMICS",
          links: [
            {
              href: "#",
              text: "Characters",
            },
            {
              href: "#",
              text: "Comics",
            },
            {
              href: "#",
              text: "Movies",
            },
            {
              href: "#",
              text: "TV",
            },
            {
              href: "#",
              text: "Games",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "News",
            },
          ],
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
/* Footer center menu*/
.footer_center_menu {
  background-image: url("@/assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  h4 {
    color: white;
  }

  ul {
    list-style: none;
    li {
      color: gray;
    }
  }

  .footer_bg_image {
    background-image: url('@/assets/img/dc-logo-bg.png');
    background-position: right;
    background-repeat: no-repeat;
  }

  .row {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    width: calc(100% / 3);
  }
}

.col-3 {
  margin-top: 2rem;
  width: calc(100% / 3);
}
</style>