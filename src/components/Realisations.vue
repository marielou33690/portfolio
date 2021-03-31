<template>
  <section id="realisations">
    <div class="contenu-realisations">
      <h2>Mes réalisations</h2>
      <ul class="nav-realisations">
        <li :class="filtreCourant == 'toutes'? 'actif' : ''" @click="filtreCourant='toutes'">//toutes</li>
        <li :class="filtreCourant == 'web'? 'actif' : ''" @click="filtreCourant='web'">//web</li>
        <li :class="filtreCourant == 'design'? 'actif' : ''" @click="filtreCourant='design'">//design</li>
        <li :class="filtreCourant == 'autres'? 'actif' : ''" @click="filtreCourant='autres'">//autres</li>
      </ul>
      <ListeProjets :listeProjets="filtrerProjets"/>
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
  data () {
    return {
      filtreCourant: 'toutes',
      classe: 'actif'
    }
  },
  computed: {
    projets() {
      return donnees.projets;
    },
    filtrerProjets() {
      const listeProjets = [];
      console.log();
      for (let i = 0; i < this.projets.length; i++) {
        if(this.filtreCourant=='toutes'){
          listeProjets.push(this.projets[i]);
        }
        else if(this.filtreCourant=='web'){
          if(this.projets[i].filtre=='web') {
          listeProjets.push(this.projets[i]);
          }
        }
        else if(this.filtreCourant=='design'){
          if(this.projets[i].filtre=='design') {
          listeProjets.push(this.projets[i]);
          }
        }
        else if(this.filtreCourant=='autres'){
          if(this.projets[i].filtre=='autres') {
          listeProjets.push(this.projets[i]);
          }
        }
        
      }
      return listeProjets;
    }
  }
}
</script>