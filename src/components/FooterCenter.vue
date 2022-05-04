<template>
  <footer class="footer_center_menu">
    <div class="footer_bg_image">
      <div class="container">
        <div class="row">
          <div
            class="col-3"
            v-for="({ title, links }, index) in footerMenu"
            :key="index"
          >
            <h4>{{ title }}</h4>
            <ul>
              <li v-for="(link, index) in links" :key="index">
                {{ link.text }}
              </li>
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
          title: "DC",
          links: [
            {
              href: "#",
              text: "Terms Of Use",
            },
            {
              href: "#",
              text: "Privacy policy(New)",
            },
            {
              href: "#",
              text: "Ad Choices",
            },
            {
              href: "#",
              text: "Advertising",
            },
            {
              href: "#",
              text: "Jobs",
            },
            {
              href: "#",
              text: "Subscriptions",
            },
            {
              href: "#",
              text: "Talent Workshops",
            },
            {
              href: "#",
              text: "CPSC Certificates",
            },
            {
              href: "#",
              text: "Ratings",
            },
            {
              href: "#",
              text: "Shop Help",
            },
            {
              href: "#",
              text: "Contact Us",
            },
          ],
        },
        {
          title: "SITES",
          links: [
            {
              href: "#",
              text: "DC",
            },
            {
              href: "#",
              text: "MAD",
            },
            {
              href: "#",
              text: "DC Kids",
            },
            {
              href: "#",
              text: "DC Universe",
            },
            {
              href: "#",
              text: "DC Power Visa",
            },
          ],
        },
        {
          title: "SHOP",
          links: [
            {
              href: "#",
              text: "Shop DC",
            },
            {
              href: "#",
              text: "Shop DC Collectibles",
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
    color: $dc-white;
  }

  ul {
    list-style: none;
    li {
      color: gray;
    }
  }

  .footer_bg_image {
    background-image: url("@/assets/img/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position-x: 91%;
    background-position-y: 53%;
    background-size: 40rem;
  }

  .row {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    width: calc(100% / 3);
    padding-bottom: 3rem;
  }
}

.col-3 {
  margin-top: 2rem;
  width: calc(100% / 3);
}
</style>