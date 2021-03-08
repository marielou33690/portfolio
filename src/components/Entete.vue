<template>
  <header class="entete">
    <div id="initiale"><a href="#accueil">mld</a></div>
    <div id="menu-burger">
            <input type="checkbox">
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <ul>
                <li class="lien-nav"><a href="#realisations">portfolio</a></li>
                <li class="lien-nav"><a href="#apropos">à propos</a></li>
            </ul>
    </div>
    <!-- <ul class="nav">
      <li><a href="#realisations">portfolio</a></li>
      <li><a href="#apropos">à propos</a></li>
       <li id="lang">
        <span>en</span>
        <span>|</span>
        <span>fr</span>
      </li>
    </ul> -->
  </header>
</template>

<script>
import "../styles/portfolio/Entete.scss";
export default {
  name: "Entete",
  // ,
  // methods: {
  //   defilement(){
  //     const barreNav = document.querySelector("nav");
  //     if (document.body.scrollTop > 80 || document.documentElement.scrollTop > 80) {
  //       barreNav.style.backgroundColor = "rgba(5,0,20,.8)";
  //   } else {
  //       barreNav.style.backgroundColor = "rgba(0,0,0,0)";
  //   }
  //   }
  // }
};
</script>