<template>
  <div id="accueil">
    <!-- Code scss à refaire pour optimiser animation Xyz, code temporaire ci-dessous -->
          <XyzTransition class="rectangle-groupe1" appear duration="5s" xyz="fade down-100% delay-2">
            <span class="rectangle-rond"></span>
          </XyzTransition>
          <XyzTransition class="rectangle-groupe1" appear duration="5s" xyz="fade down-100% delay-2">
            <span class="rectangle-rond"></span>
          </XyzTransition>
          <XyzTransition class="rectangle-groupe1" appear duration="5s" xyz="fade down-100% delay-5">
            <div class="contenu-accueil">
            <h1>Salut,</h1> <br>
            <div class="nom"><h1>Je suis</h1><h1>Marie-Lou</h1></div>
            <h2>une stagiaire en programmation web</h2>
            <!-- <button class="bouton">rejouer</button> -->
          </div>
          </XyzTransition>
          <XyzTransition class="rectangle-groupe1" appear duration="5s" xyz="fade down-100% delay-2">
            <span class="rectangle-rond"></span>
          </XyzTransition>
          <XyzTransition class="rectangle-groupe1" appear duration="5s" xyz="fade down-100% delay-2">
            <span class="rectangle-rond"></span>
          </XyzTransition>
          <XyzTransition class="rectangle-groupe1" appear duration="5s" xyz="fade down-100% delay-2">
            <span class="rectangle-rond"></span>
          </XyzTransition>
  </div>
</template>

<script>
// Import the functions/mixins
import '@animxyz/core';
import "../styles/portfolio/Accueil.scss";
export default {
  name: 'Accueil'
}
</script>
