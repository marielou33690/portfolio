<template>
<!-- Temporaire pour faire css du lightbox -->
<div></div>
  <!-- <div id="lightbox">
    <div id="contenu-lightbox">
      <button>g</button>
      <img :src="require('../assets/images/lightbox_construction.jpg')" alt="">
      <button>></button>
      <div class="carte">
        <h1>Nom du projet</h1>
        <h2>Technologies utilis/es</h2>
        <p>desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc desc</p>
        <button>Aller au site</button>
      </div>
    </div>
  </div> -->
</template>

<script>
import "../styles/portfolio/Lightbox.scss";
export default {
  name: 'Lightbox'
  // ,
  // props:{
  //   thumbnails:{
  //     type: String,
  //     required: true
  //   },
  //   images:{
  //     type: Array,
  //     required: true
  //   }
  // },
  // data(){
  //   return{
  //     visible: false,
  //     index: 0
  //   }
  // },
  // methods: {
  //   show(){
  //     this.visible = true;
  //   },
  //   hide(){
  //     this.visible = false;
  //     this.index = 0
  //   }
  // }
}
</script>
