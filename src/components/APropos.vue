<template>
  <section id="apropos">
    <div class="contenu-apropos">
      <h2>À propos</h2>
      <div class="qualites">
        <div>
          <img src="../assets/images/icones/eclair.png" alt="">
          <p>Apprend rapidement</p>
        </div>
        <div>
          <img src="../assets/images/icones/ampoule.png" alt="">
          <p>Proactive</p>
        </div>
        <div>
          <img src="../assets/images/icones/equipe.png" alt="">
          <p>Esprit d'équipe</p>
        </div>
      </div>
      <div class="description">
        <img src="../assets/images/MarieLou.jpg" alt="">
        <div class="informations">
          <p>Je suis une finissante en technique d'intégration multimédia.
              J'y ai découvert que j'aime beaucoup la programmation à
              travers ce programme. C'est pour ça que j'ai décidé de poursuivre mes études au Bac en Informatique. J'adore résoudre des  problèmes de
              manière créative et j'apprends très rapidement. J'ai hâte de 
              pouvoir travailler dans une équipe de gens passionnés par
              leur travail.
          </p>
          <!-- <button @click="lireFichier">Mon CV</button> -->
          <p>marielou33690@gmail.com</p>
          <p>Montréal, QC, Canada</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import "../styles/portfolio/APropos.scss";
export default {
  name: 'APropos'
  // ,
  // methods: {
  //   lireFichier() {
  //    window.open(('https://www.facebook.com/', '_blank')) //to open in new tab
  //  }
  // }
}
</script>