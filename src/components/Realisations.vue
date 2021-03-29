<template>
  <section id="realisations">
    <div class="contenu-realisations">
      <h2>Mes réalisations</h2>
      <ul class="nav-realisations">
        <!-- <li class="actif">//toutes</li>
        <li>//web</li>
        <li>//design</li>
        <li>//autres</li> -->
      </ul>
      <ListeProjets :listeProjets="projets"/>
      </div>
  </section>
</template>

<script>

import donnees from '../assets/data.json'
import "../styles/portfolio/Realisations.scss";
import ListeProjets from './ListeProjets'
export default {
  name: 'Realisation',
  components: {
    'ListeProjets' : ListeProjets
  },
  computed: {
    projets() {
      return donnees.projets;
    }
  }
}
</script>