<template>
  <div class="">
    <Navbar/>
    <Typewriter/>
    <div class="review-section mt-5 mx-auto content-card w-fit-content">
      <h2>Bei Amazon bestellen oder bei Kindle lesen</h2>
      <div class="d-flex justify-content-around w-100">
        <a class="btn btn-outline-warning" target="_blank" href="https://www.amazon.de/Aufbruch-nach-Honua-Reinhard-L%C3%B6chner/dp/B09HG6HNB8/ref=sr_1_2?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&dchild=1&keywords=honua&qid=1634130532&sr=8-2">Buch Bestellen</a>
        <a class="btn btn-warning" target="_blank" href="https://www.amazon.de/Aufbruch-nach-Honua-Utopischer-Roman-ebook/dp/B09HHR8ZCJ/ref=tmm_kin_swatch_0?_encoding=UTF8&qid=1634130532&sr=8-2">Bei Kindle lesen</a>
      </div>
    </div>
    <div class="review-section mt-5 mx-auto content-card w-fit-content">
      <h2>Interview mit Buchszene.de</h2>
      <p>
        Die Menschheit hat die Erde an den Rand des Zusammenbruchs gebracht. Deshalb fliegt eine Crew genetisch modifizierter Menschen ins All. <br>
        Reinhard Löchner im Interview über seinen Roman „Aufbruch nach Honua“.
      </p>
      <div class="d-flex justify-content-around w-100">
        <a class="btn btn-outline-success" target="_blank" href="https://buchszene.de/aufbruch-nach-honua-interview/">Zum Interview</a>
      </div>
    </div>
    <div class="d-flex flex-column">
      <Review v-for='review in reviews' :key="review.id" :review="review"/>
    </div>
    <div class="review-section mt-5 mx-auto content-card w-fit-content">
      <h2>Ihre Meinung ist uns wichtig!</h2>
      <p>Sie haben das Buch schon gelesen? Dann würden wir uns sehr über eine Bewertung freuen.</p>
      <a class="btn btn-success" target="_blank" href="https://www.amazon.de/review/create-review/ref=cm_cr_othr_d_wr_but_top?ie=UTF8&channel=glance-detail&asin=B09HG6HNB8">Jetzt Bewerten</a>
    </div>
    <div style="height: 3rem"></div>
  </div>
</template>

<script>
  import json from 'assets/reviews.json'
  export default{
    data(){
      return{
        reviews: json
      }
    }
  }
</script>

<style>
</style>
