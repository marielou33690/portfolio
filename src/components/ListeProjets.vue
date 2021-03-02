<template>
 <ul class="liste-projets">
   <li v-for="projet in projets"  v-bind:projet="projet" :key="projet.titre">
     {{projet.titre}}
     <img :src="projet.src" :alt="projet.alt">
   </li>
 </ul>
</template>

<script>
import "../styles/portfolio/ListeProjets.scss";
export default {
  name: 'ListeProjets',
  data() {
    return{
      projets: [
        {
          titre: "Refonte TIM",
          src: require("../assets/images/projets/refonteTim.jpg"),
          alt: "Projet de refonte du site tim",
          techno: "HTML, SCSS, JS,  PHP"
        },
        {
          titre: "Quiz sur la bouffe",
          src: require("../assets/images/projets/quizBouffe.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Refonte Roman Emporium",
          src: require("../assets/images/projets/refonteRoman.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Jeu Évasion",
          src: require("../assets/images/projets/jeuEvasion.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Chaîne YouTube",
          src: require("../assets/images/projets/chaineYoutube.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Vaisseau 3D",
          src: require("../assets/images/projets/vaisseau3D.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Matte Painting",
          src: require("../assets/images/projets/mattePainting.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Affiche Ocean Cleanup",
          src: require("../assets/images/projets/oceanCleanup.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
      ]
    }
  }
}
</script>