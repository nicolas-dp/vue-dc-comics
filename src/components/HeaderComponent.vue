<template>
  <header>
      <div class="container">
        <nav class="logo_navabar">
          <div class="logo">
            <img style="height: 70px;" src="@/assets/img/dc-logo.png" alt="..." />
          </div>
          <div class="menu">
            <a :href="item.href" v-for="item in menu" :key="item.id">{{item.link}}</a>
          </div>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
  name: 'SiteHeader',
  data(){
    return{
      menu: [
        {
          id: 1,
          href: '#',
          link: 'characters'
        },
        {
          id: 2,
          href: '#',
          link: 'comics'
        },
        {
          id: 3,
          href: '#',
          link: 'movies'
        },
        {
          id: 4,
          href: '#',
          link: 'tv'
        },
        {
          id: 5,
          href: '#',
          link: 'games'
        },
        {
          id: 6,
          href: '#',
          link: 'collectibles'
        },
        {
          id: 7,
          href: '#',
          link: 'videos'
        },
        {
          id: 8,
          href: '#',
          link: 'fans'
        },
        {
          id: 9,
          href: '#',
          link: 'news'
        },
        {
          id: 10,
          href: '#',
          link: 'shop'
        }

      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scope>
  /* Site Header */

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
    border-bottom: 3px solid #0282F9;
;
  }
}
</style>
