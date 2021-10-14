<template>
  <div>
    <main class="wrapper">
      <section class="section parallax earth-bg">
        <Nuxt/>
      </section>
    </main>
    <Footer/>
  </div>
</template>

<script>
</script>

<style>
  body {
    background: #000;
  }

  .wrapper {
    height: 100vh;
    overflow-x: hidden;
    overflow-y: auto;
    perspective: 2px;
  }

  .section {
    position: relative;
    height: 300vh;
  }

  .parallax::after {
    content: " ";
    position: absolute;
    top: 30vh;
    right: 0;
    bottom: 0;
    left: 0;

    transform: translateZ(-1px) scale(1.5);
    background-size: cover;
    background-position: top;
    z-index: -1;
  }

  .earth-bg::after {
    background-image: url('~assets/earth.jpeg');
  }

  .content-card {
    color: #FFF;
    background: #0009;
    margin: 1rem;
    padding: 1rem;
    border-radius: 1rem;
  }

  .w-fit-content {
    width: -moz-fit-content;
    width: fit-content;
  }
</style>
