<template>
  <header class="entete">
    <div @click="navActif='accueil'" id="initiale"><a href="#accueil">mld</a></div>
    <div id="menu-burger">
            <input type="checkbox">
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <ul>
                <li @click="navActif='realisations'" class="lien-nav"><a :class="navActif == 'realisations'? 'nav-actif' : ''" href="#realisations">portfolio</a></li>
                <li @click="navActif='aPropos'" class="lien-nav"><a :class="navActif == 'aPropos'? 'nav-actif' : ''" href="#apropos">à propos</a></li>
            </ul>
    </div>
       <!-- <li id="lang">
        <span>en</span>
        <span>|</span>
        <span>fr</span>
      </li> -->
  </header>
</template>

<script>
import "../styles/portfolio/Entete.scss";
export default {
  name: "Entete",
  data () {
    return{
      navActif:''
    }
  }
};
</script>