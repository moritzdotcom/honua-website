<template>
  <nav class="navbar navbar-expand-lg position-sticky">
    <div class="container-fluid">
      <nuxt-link class="navbar-brand" to="/">Home</nuxt-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <nuxt-link class="nav-link" :class="page == 'book' ? 'active' : ''" to="/book">Honua</nuxt-link>
          <nuxt-link class="nav-link" :class="page == 'author' ? 'active' : ''" to="/author">Autor</nuxt-link>
          <a class="nav-link btn btn-outline-success text-success" target="_blank" href="https://www.amazon.de/Aufbruch-nach-Honua-Reinhard-L%C3%B6chner-ebook/dp/B09HHR8ZCJ/ref=tmm_kin_swatch_0?_encoding=UTF8&qid=1633005611&sr=8-2">Jetzt Kaufen</a>
        </div>
      </div>
    </div>
  </nav>
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
