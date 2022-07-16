<template>
  <header>
    <!--     <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container">
        <a class="navbar-brand" href="#home">
          <img height="70" src="@/assets/img/dc-logo.png" alt="" />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav">
            <li
              class="nav-item border_bottom"
              v-for="item in menu"
              :key="item.id"
            >
              <a :href="item.href">{{ item.link }}</a>
            </li>
          </ul>
        </div>
      </div>
    </nav> -->

    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img height="50" src="@/assets/img/dc-logo.png" alt="" />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item border_bottom" v-for="item in menu"
              :key="item.id">
              <a class="nav-link active" aria-current="page" :href="item.href">{{ item.link }}</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

  </header>
</template>

<script>
export default {
  name: "SiteHeader",
  data() {
    return {
      menu: [
        {
          id: 1,
          href: "#",
          link: "characters",
        },
        {
          id: 2,
          href: "#",
          link: "comics",
        },
        {
          id: 3,
          href: "#",
          link: "movies",
        },
        {
          id: 4,
          href: "#",
          link: "tv",
        },
        {
          id: 5,
          href: "#",
          link: "games",
        },
        {
          id: 6,
          href: "#",
          link: "collectibles",
        },
        {
          id: 7,
          href: "#",
          link: "videos",
        },
        {
          id: 8,
          href: "#",
          link: "fans",
        },
        {
          id: 9,
          href: "#",
          link: "news",
        },
        {
          id: 10,
          href: "#",
          link: "shop",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scope>
/* Site Header */



.border_bottom {
  padding: 1rem;
  &:hover {
    border-bottom: 4px solid $dc-primary;
  }
}

a {
  text-decoration: none;
  color: $dc-main-bg;
  text-transform: uppercase;
}
</style>
