<template>
  <div class="Accueil">
      <span class="rectangle-rond"></span>
      <!-- <span class="rectangle-rond"></span> -->
      <h1>Salut,</h1> <br>
      <div class="nom"><h1>Je suis</h1><h1>Marie-Lou</h1></div>
    
    <!-- <h1><span>Salut,</span> 
      <br>
      <span>Je suis</span> 
      <span>Marie-Lou</span>
    </h1> -->
    <h2>une stagiaire en programmation web</h2>
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

h1{
  margin: 0;
  font-family: 'Staatliches', cursive;
  font-size: 4em;
  justify-content: center;
  align-items: center;
  display: flex;
  margin: 0 auto;
  text-align: center;
}

/* h1 span:first-child{
 
}
h1 span:nth-of-type(2)
{
  
  padding: 80px 0 0 10px;
}*/

h1::after{
  
  color: #BCFDFF;
  padding: 80px 0 0 10px;
} 
span{
  font-size: 4em;
}
.nom{
  display: flex;
  width: 50vw;
  margin: 0 auto;
}

.nom h1:nth-of-type(2){
   color: #BCFDFF;
}

.rectangle-rond{
  background-color: #FC6478;
  border-radius: 30px;
  width: 200px;
  height: 60px;
  display: block;
  transform: rotate(40deg);
}
</style>
