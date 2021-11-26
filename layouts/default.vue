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

  h1, h2, h3, h4, h5, p {
    /* Font minimum, preferred and maximum value */
    font-size: clamp(var(--min), var(--val), var(--max));
  }

  /* Font size variables */
  h1 {
    --min: 2em; /* minimum value */
    --val: 4vw; /* preferred value = 5% viewport width */
    --max: 3em; /* maximum value */
  }
  h2 {
    --min: 1.8em;
    --val: 3.8vw;
    --max: 2.8em;
  }
  h3 {
    --min: 1.6em;
    --val: 3.6vw;
    --max: 2.6em;
  }
  h4 {
    --min: 1.4em;
    --val: 3.4vw;
    --max: 2.4em;
  }
  h5 {
    --min: 1.2em;
    --val: 2.2vw;
    --max: 2.2em;
  }
  p {
    --min: 1em;
    --val: 2vw;
    --max: 2em;
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
