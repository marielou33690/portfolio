<template>
  <div id="app">
    <Chargement />
    <Entete/>
    <section class="contenuPrincipal">
      <Accueil/>
      <Realisations />
      <!-- <Lightbox /> -->
      <APropos/>
    </section>
    <PiedDePage/>
    
  </div>
</template>

<script>
import Chargement from './components/Chargement.vue'
import Accueil from './components/Accueil.vue'
import Entete from './components/Entete.vue'
import Realisations from './components/Realisations.vue'
// import Lightbox from './components/Lightbox.vue'
import PiedDePage from './components/PiedDePage.vue'
import APropos from './components/APropos.vue'

// Styles communs
import "./styles/general/_box-sizing.scss";
import "./styles/general/_normalize.scss";
import "./styles/portfolio/Commun.scss";

export default {
  name: 'App',
  // props:{
  //   lightboxActif: {
  //     type: Boolean,
  //     default: true
  //   }
  // },
  components: {
    Chargement,
    Accueil,
    Entete,
    Realisations,
    // Lightbox,
    APropos,
    PiedDePage
  }
  // ,
  // data() {
  //   return{
  //     images: [
  //       require("./assets/images/projets/prj01-cover.jpg"),
  //       require("./assets/images/projets/prj02-cover.jpg"),
  //       require("./assets/images/projets/prj03-cover.jpg"),
  //       require("./assets/images/projets/prj05-cover.jpg"),
  //       require("./assets/images/projets/prj06-cover.jpg"),
  //       require("./assets/images/projets/prj07-cover.jpg"),
  //       require("./assets/images/projets/prj08-cover.jpg")
  //     ]
  //   }
  // }
}
</script>