<template>
  <div id="lightbox" @click="toggle">
      <div id="contenu-lightbox" @click.stop>
        <div class="image">
          <button @click="precedent"></button>
          <img :src="require(`../assets/images/projets/prj${compteur}.jpg`)" :alt="infosProjet.listeProjets[compteur].alt">
          <button @click="suivant">></button>
        </div>
        <div class="carte">
          <h2>{{infosProjet.listeProjets[compteur].titre}}</h2>
          <h3>{{infosProjet.listeProjets[compteur].techno}}</h3>
          <p>{{infosProjet.listeProjets[compteur].desc}}</p>
          <div class="boutons">
            <button v-if="infosProjet.listeProjets[compteur].url" @click="ouvrirLien" class="btn-site">Aller au site</button>
            <button class="btn-fermer" @click="toggle">X</button>
          </div>
        </div>
      </div>
    </div>
</template>

<script>

import "../styles/portfolio/Lightbox.scss";
export default {
  name: 'Lightbox',
  props: ['lightboxActif', 'value', 'infosProjet'],
  data() {
    return{
      compteur : this.infosProjet.idCourant
    }
  },
  methods: {
    toggle: function (value) {
      this.$emit('input', value);
    },
    suivant: function() {
      this.compteur < this.infosProjet.listeProjets.length ? this.compteur += 1 : this.compteur = 0;
      console.log('click suivant', this.compteur);
      return this.$emit('suivant');
    },
    precedent: function() {
      this.compteur > 0 ? this.compteur -= 1 : this.compteur = this.infosProjet.listeProjets.length-1;
      console.log('click précédent', this.compteur);
      return this.$emit('précédent');
    },
    ouvrirLien: function () {   
          window.open(this.infosProjet.listeProjets[this.compteur].url, "_blank");    
      }
  }
}
</script>
