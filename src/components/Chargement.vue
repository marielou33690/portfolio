<template>
  <div id="chargement" v-if="!isloaded">
    <div class="rond"></div>
    <div class="rond"></div>
    <div class="rond"></div>
    <div class="rond"></div>
  </div>
</template>

<script>
import "../styles/portfolio/Chargement.scss";
export default {
  name: 'Chargement',
  data: () => {
    return{
      isloaded: false
    }
  },
  mounted(){
    document.onreadystatechange = () => {
      if(document.readyState == "complete"){
        this.isloaded = true;
      }
    }
  }
}
</script>
