<template>
  <b-navbar toggleable="lg" type="dark" variant="" class="position-sticky">
    <nuxt-link class="navbar-brand" to="/">Home</nuxt-link>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <nuxt-link class="nav-link" :class="page == 'book' ? 'active' : ''" to="/book">Aufbruch nach Honua</nuxt-link>
        <nuxt-link class="nav-link flex-grow-1" :class="page == 'author' ? 'active' : ''" to="/author">Autor</nuxt-link>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <a class="nav-link btn btn-outline-success text-success" target="_blank" href="https://www.amazon.de/Aufbruch-nach-Honua-Reinhard-L%C3%B6chner-ebook/dp/B09HHR8ZCJ/ref=tmm_kin_swatch_0?_encoding=UTF8&qid=1633005611&sr=8-2">Jetzt Kaufen</a>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
  export default {
    props: ['page']
  }
</script>

<style>
  .navbar {
    top: 0;
    background: #0009;
  }

  .navbar-brand {
    color: white;
  }
  .nav-link {
    color: white;
  }
</style>
