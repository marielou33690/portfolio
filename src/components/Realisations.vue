<template>
  <section class="realisations">
    <div class="contenu-realisations">
      <h1>Mes réalisations</h1>
      <ul class="nav-realisations">
        <li class="actif">//toutes</li>
        <li>//web</li>
        <li>//design</li>
        <li>//autres</li>
      </ul>
      <ListeProjets/>
      </div>
  </section>
</template>

<script>
import "../styles/portfolio/Realisations.scss";
import ListeProjets from './ListeProjets'
export default {
  name: 'Realisation',
  components: {
    'ListeProjets' : ListeProjets
  }
}
</script>