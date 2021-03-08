<template>
<div>
  <ul class="liste-projets">
    <li v-for="projet in projets"  v-bind:projet="projet" :key="projet.titre" @click="lightboxActif=true">
      <div class="superposition">
          <h2>{{projet.titre}}</h2>
          <p>{{projet.techno}}</p>
        </div>
      <img :src="projet.src" :alt="projet.alt">
    </li>
  </ul>

  <!-- Temporaire pour faire css du lightbox -->
  <div id="lightbox" v-if="lightboxActif==true">
      <div id="contenu-lightbox">
        <div class="image">
          <button></button>
          <img :src="require('../assets/images/lightbox_construction.jpg')" alt="">
          <button>></button>
        </div>
        <div class="carte">
          <h1>Nom du projet</h1>
          <h2>HTML, SCSS, JS,  PHP</h2>
          <p>desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc</p>
          <div class="boutons">
            <button class="btn-site">Aller au site</button>
            <button class="btn-fermer" @click="lightboxActif=false">X</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import "../styles/portfolio/ListeProjets.scss";
// Temporaire pour faire css du lightbox
import "../styles/portfolio/Lightbox.scss";
export default {
  name: 'ListeProjets',
  data() {
    return{
      // Temporaire pour faire css du lightbox
      lightboxActif: false,
      isAddClass: false,
      methods: {
            addClass: function() {
                this.isAddClass = true;
        }
    },
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