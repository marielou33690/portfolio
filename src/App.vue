<template>
  <div id="app">
    <Chargement />
    <Entete/>
    <section class="contenuPrincipal">
      <Accueil/>
      <Realisations />
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
  components: {
    Chargement,
    Accueil,
    Entete,
    Realisations,
    APropos,
    PiedDePage
  }
}
</script>