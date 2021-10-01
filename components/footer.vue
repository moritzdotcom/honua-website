<template>
  <div class="footer position-fixed d-flex justify-content-center">
    <a class="footer-link" target="_blank" href="https://www.instagram.com/ray_loechner/"><b-icon icon="instagram"></b-icon></a>
    <a class="footer-link" target="_blank" href="https://www.facebook.com/reinhard.loechner/"><b-icon icon="facebook"></b-icon></a>
    <a class="footer-link" target="_blank" href="https://www.linkedin.com/in/reinhard-l%C3%B6chner-a45200/"><b-icon icon="linkedin"></b-icon></a>
    <a class="footer-link" target="_blank" href="https://www.xing.com/profile/Reinhard_Loechner/cv"><XingLogo/></a>
  </div>
</template>

<script>
  import { BIcon, BIconLinkedin, BIconFacebook, BIconInstagram } from 'bootstrap-vue'
  import 'bootstrap-vue/dist/bootstrap-vue-icons.min.css'

  export default {
    components: {
      BIcon,
      BIconLinkedin,
      BIconFacebook,
      BIconInstagram
    }
  }
</script>

<style>
  .footer {
    font-size: 1.5em;
    bottom: 0;
    width: 100%;
    background: #0009;
  }

  .footer-link {
    padding: 0.5rem 2rem;
    color: white;
    font-family: monaco;
    cursor: pointer;
  }

  .footer-link:hover {
    color: #27A744;
    text-decoration: none;
  }
</style>
