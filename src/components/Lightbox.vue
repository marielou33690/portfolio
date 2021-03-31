<template>
  <div id="lightbox" @click="infosProjet.fermerLightbox">
      <div id="contenu-lightbox" @click.stop>
        <div class="image">
          <button @click="precedent"></button>
          <!-- Avec compteur -->
          <img :src="require(`../assets/images/projets/prj${compteur}.jpg`)" :alt="infosProjet.listeProjets[compteur].alt">
          <button @click="suivant">></button>
        </div>
        <div class="carte">
          <h2>{{infosProjet.listeProjets[compteur].titre}}</h2>
          <h3>{{infosProjet.listeProjets[compteur].techno}}</h3>
          <p>{{infosProjet.listeProjets[compteur].desc}}</p>
          <div class="boutons">
            <button v-if="infosProjet.listeProjets[compteur].url" @click="ouvrirLien" class="btn-site">Aller au site</button>
            <button class="btn-fermer" @click="infosProjet.fermerLightbox">X</button>
          </div>
        </div>
      </div>
    </div>
</template>

<script>

import "../styles/portfolio/Lightbox.scss";
export default {
  name: 'Lightbox',
  props: ['infosProjet', 'fermerLightbox'],
  data() {
    return{
      compteur : this.infosProjet.idCourant
    }
  },
  methods: {
    suivant: function() {
      this.compteur < this.infosProjet.listeProjets.length-1 ? this.compteur += 1 : this.compteur = 0;
      console.log('click suivant', this.compteur);
    },
    precedent: function() {
      this.compteur > 0 ? this.compteur -= 1 : this.compteur = this.infosProjet.listeProjets.length-1;
      console.log('click précédent', this.compteur);
    },
    ouvrirLien: function () {   
          window.open(this.infosProjet.listeProjets[this.compteur].url, "_blank");    
      }
  }
}
</script>
