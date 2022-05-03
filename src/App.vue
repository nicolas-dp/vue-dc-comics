<template>
  <div id="app">
    <header>
      <div class="container">
        <nav class="logo_navabar">
          <div class="logo">
            <img src="@/assets/img/dc-logo.png" alt="..." />
          </div>
          <div class="menu">
            <a href="#">characters</a>
            <a href="#">comics</a>
            <a href="#">movies</a>
            <a href="#">tv</a>
            <a href="#">games</a>
            <a href="#">collectibles</a>
            <a href="#">videos</a>
            <a href="#">fans</a>
            <a href="#">news</a>
            <a href="#">shop</a>
          </div>
        </nav>
      </div>
    </header>

    <main>
      <div class="container">
        <h1>-- Content goes here --</h1>
      </div>
    </main>

    <footer>
      <div class="container">
        <div class="footer_menu">
          <a href="#">
            <img height="90" src="@/assets/img/buy-comics-digital-comics.png" alt="..." />
            <span>digital comics</span>
          </a>

          <a href="#">
            <img height="90" src="@/assets/img/buy-comics-merchandise.png" alt="..." />
            <span>dc merchandise</span>
          </a>

          <a href="#">
            <img height="90" src="@/assets/img/buy-comics-subscriptions.png" alt="..." />
            <span>subscription</span>
          </a>

          <a href="#">
            <img height="90" src="@/assets/img/buy-comics-shop-locator.png" alt="..." />
            <span>comic shop locator</span>
          </a>

          <a href="#">
            <img style="height: 60px;" src="@/assets/img/buy-dc-power-visa.svg" alt="..." />
            <span>dc power visa</span>
          </a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
/* import HelloWorld from './components/HelloWorld.vue' */

export default {
  name: "App",
  components: {
    /* HelloWorld */
  },
};
</script>

<style lang="scss">
#app {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50; */
}

/* Common */

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

img {
  max-width: 100%;
}

/* Utilities */
.container {
  width: 1400px;
  margin: 0 auto;
}

/* Site Header */

header {
  height: 130px;
}

.logo_navabar {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
}

a {
  text-decoration: none;
  color: black;
  padding: 0.5rem;
  text-transform: uppercase;

  &:hover {
    border-bottom: 3px solid rgb(2, 2, 168);
  }
}

/* Site Main */

main {
  color: white;
  background-color: #1c1c1c;
  height: 20vh;
}

/* Site Footer */

footer {
  background-color: #0282f9;
}

.footer_menu {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding: 1rem;

  &>a {
    color: white;
    display: flex;
    border: none;
    align-items: center;
    flex-wrap: wrap;
    padding: 0.7rem;
  }
}
</style>
