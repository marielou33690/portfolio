<template>
  <div class="Accueil">
    <span class="rectangle-rond"></span>
    <span class="rectangle-rond"></span>
    <div class="contenu-accueil">
      
      <h1>Salut,</h1> <br>
      <div class="nom"><h1>Je suis</h1><h1>Marie-Lou</h1></div>
    <!-- <h1><span>Salut,</span> 
      <br>
      <span>Je suis</span> 
      <span>Marie-Lou</span>
    </h1> -->
    <h2>une stagiaire en programmation web</h2>
    </div>
    <!-- <span class="rectangle-rond"></span>
    <span class="rectangle-rond"></span>
    <span class="rectangle-rond"></span> -->
  </div>
</template>

<script>
import "../styles/portfolio/Accueil.scss";
export default {
  name: 'Accueil',
  props: {
    msg: String
  }
}
</script>
