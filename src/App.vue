<template>
  <div id="app">
    <Entete/>
    <section class="contenuPrincipal">
      <Accueil msg="Welcome to Your Vue.js App"/>
      <Realisations/>
      <APropos/>
    </section>
    <PiedDePage/>
    
  </div>
</template>

<script>
import Accueil from './components/Accueil.vue'
import Entete from './components/Entete.vue'
import Realisations from './components/Realisations.vue'
import PiedDePage from './components/PiedDePage.vue'
import APropos from './components/APropos.vue'
import "./styles/portfolio/Commun.scss";

export default {
  name: 'App',
  components: {
    Accueil,
    Entete,
    Realisations,
    APropos,
    PiedDePage
  }
}
</script>