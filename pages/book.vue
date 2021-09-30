<template>
  <div class="page-content">
    <Navbar page="book"/>
    <div class="content-card">
      <h1>Das Buch</h1>
      <p>Die Klimaerwärmung hat die Menschheit zum Handeln gezwungen. Nach Überschwemmungen, Flüchtlingselend und einem vernichtenden Krieg lebt sie nun in 400 selbständigen Metropolen und in einer nachhaltigen, freiheitlichen Weltordnung. Die Beinahe-Kollision mit einem riesigen Asteroiden zeigt jedoch, dass die Menschheit weiterhin in Gefahr schwebt, ausgelöscht zu werden. Deswegen wird im Jahr 2061 die „Mission Atlantis“ ins Leben gerufen: der Aufbruch ins All als gemeinsame Anstrengung aller Metropolen. 37 Jahre später startet die erste Crew mit dem Raum-schiff Atlantis zum 30.000 Lichtjahre entfernten Planeten Honua, der beste Aussichten auf eine Kolonisierung bietet. Sieben genetisch modifizierte Menschen verlassen auf der Atlantis die Erde und lassen alles zurück, um weit draußen im All eine neue Zivilisation zu erschaffen, die die Fehler der alten möglichst nicht wiederholen soll …</p>
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
