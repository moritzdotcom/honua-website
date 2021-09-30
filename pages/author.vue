<template>
  <div class="page-content">
    <Navbar page="author"/>
    <div class="content-card">
      <h1>Der Autor</h1>
      <p>Reinhard Löchner, der am 8. Oktober 1964 in Köln geboren wurde, ist verheiratet und hat vier Kinder. Nach dem Abschluss seines Studiums zum Dipl.-Wirtsch.-Ing. an der Technischen Universität Darmstadt führten ihn berufliche Stationen im technologiegetriebenen Mittelstand über einen Großkonzern zum Venture Capital. Ab dem Jahr 2000 war er am Aufbau zahlreicher Unternehmen der Solar- und Windenergie maßgeblich beteiligt. Heute lebt er als erfolgreicher Unternehmer in Düsseldorf und widmet sich in seiner Freizeit der Schriftstellerei. Bei dem vorliegenden utopischen Roman «Aufbruch nach Honua» handelt es sich um sein Erstlingswerk. Die Abenteuer der Crew auf Honua sind aber noch lange nicht zu Ende. Seien sie gespannt. Die Gedanken sind frei. Vielen Dank für ihr Interesse und ihre Weiterempfehlung.</p>
    </div>
    <Footer/>
  </div>
</template>

<script>
export default {}
</script>

<style>
  .page-content {
    background: url('~assets/earth.jpeg');
    height: 300vh;
    background-size: cover;
    background-position: center;
  }

  .content-card {
    color: #FFF;
    background: #0009;
    margin: 1rem;
    padding: 1rem;
    border-radius: 1rem;
  }
</style>
