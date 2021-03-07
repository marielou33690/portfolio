<template>
 <ul class="liste-projets">
   <li v-for="projet in projets"  v-bind:projet="projet" :key="projet.titre">
     <div class="superposition">
        <h2>{{projet.titre}}</h2>
        <p>{{projet.techno}}</p>
       </div>
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
          src: require("../assets/images/projets/prj01-cover.jpg"),
          alt: "Projet de refonte du site tim",
          techno: "HTML, SCSS, JS,  PHP"
        },
        {
          titre: "Quiz sur la bouffe",
          src: require("../assets/images/projets/prj02-cover.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Refonte Roman Emporium",
          src: require("../assets/images/projets/prj03-cover.jpg"),
          alt: "Quiz en javascript",
          techno: "HTML, CSS, JS"
        }
        ,
        {
          titre: "Jeu Évasion",
          src: require("../assets/images/projets/prj04-cover.jpg"),
          alt: "Quiz en javascript",
          techno: "Phaser, HTML, CSS, JS"
        }
        ,
        {
          titre: "Chaîne YouTube",
          src: require("../assets/images/projets/prj05-cover.jpg"),
          alt: "Quiz en javascript",
          techno: "Premiere, Photoshop"
        }
        ,
        {
          titre: "Vaisseau 3D",
          src: require("../assets/images/projets/prj06-cover.jpg"),
          alt: "Quiz en javascript",
          techno: "Maya, Photoshop"
        }
        ,
        {
          titre: "Matte Painting",
          src: require("../assets/images/projets/prj07-cover.jpg"),
          alt: "Quiz en javascript",
          techno: "Photoshop"
        }
        ,
        {
          titre: "Affiche Ocean Cleanup",
          src: require("../assets/images/projets/prj08-cover.jpg"),
          alt: "Quiz en javascript",
          techno: "Photoshop"
        }
      ]
    }
  }
}
</script>