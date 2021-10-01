<template>
  <div class="footer position-fixed d-flex justify-content-center">
    <a class="footer-link" target="_blank" href="https://www.facebook.com/reinhard.loechner/">Facebook</a>
    <a class="footer-link" target="_blank" href="https://www.linkedin.com/in/reinhard-l%C3%B6chner-a45200/">LinkedIn</a>
    <a class="footer-link" target="_blank" href="https://www.xing.com/profile/Reinhard_Loechner/cv">Xing</a>
  </div>
</template>

<script>
  export default {
  }
</script>

<style>
  .footer {
    bottom: 0;
    width: 100%;
    background: #0009;
  }

  .footer-link {
    padding: 1rem 2rem;
    color: white;
    font-family: monaco;
    cursor: pointer;
  }

  .footer-link:hover {
    color: green;
    text-decoration: none;
  }
</style>
