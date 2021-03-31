<template>
<div>
  <ul class="liste-projets">
    <li :projet="projet" v-for="projet in listeProjets" :key="projet.id" @click="lightboxActif=true, idCourant=projet.id">
      <div class="superposition">
          <h2>{{projet.titre}}</h2>
          <p>{{projet.techno}}</p>
        </div>
      <img :src="require(`../assets/images/projets/prj${projet.id}-cover.jpg`)" :alt="projet.alt">
    </li>
  </ul>
  <transition name="fondu">
    <Lightbox v-if="lightboxActif==true" :infosProjet="{idCourant: idCourant, listeProjets: listeProjets, fermerLightbox:fermerLightbox}"/>
  </transition>
  </div>
</template>

<script>
import "../styles/portfolio/ListeProjets.scss";
import Lightbox from './Lightbox.vue'
import "../styles/portfolio/Lightbox.scss";
export default {
  name: 'ListeProjets',
  components: {
    'Lightbox' : Lightbox
  },
  props: ['listeProjets'],
  data() {
    return{
      lightboxActif: false,
      idCourant: ''
    }
  },
  methods: {
    fermerLightbox(){
      this.lightboxActif = false;
    }
  },
  watch: {
    lightboxActif: function() {
      console.log(document.documentElement.style.overflow);
      console.log(this.lightboxActif);
      if(this.lightboxActif == true){
        document.documentElement.style.overflow = 'hidden'
        return
      }
      document.documentElement.style.overflow = null
    }
  }
}
</script>