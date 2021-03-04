<template>
  <header class="entete">
    <div id="initiale">
      mld
    </div>
    <ul class="nav" v-on:scroll="defilement">
      <li>portfolio</li>
      <li>à propos</li>
      <li>contact</li>
      <li id="lang">
        <span>en</span> 
        <span>|</span>
        <span>fr</span>
      </li>
    </ul>

  </header>
</template>

<script>
import "../styles/portfolio/Entete.scss";
export default {
  name: 'Entete'
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
}
</script>