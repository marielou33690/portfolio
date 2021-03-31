<template>
  <footer class="pied-page">
    <div id="signature">
      Marie-Lou Denis
    </div>
    <div id="footer-contact">
      <h2>Contact</h2>
      <div class="infosLongues">
        <p>marielou33690@gmail.com</p>
        <a target= "_blank" href="https://www.linkedin.com/in/marie-lou-denis-61bbb71ba/">Mon LinkedIn</a>
      </div>
      <div class="infosIcones">
        <img src="../assets/images/icones/linkedIn.png" alt="">
        <div>
          <a target= "_blank" href="https://www.linkedin.com/in/marie-lou-denis-61bbb71ba/"></a>
          <img src="../assets/images/icones/email.png" alt="">
        </div>
      </div>
    </div>
    <div id="footer-apropos">
      <h2>À propos</h2>
      <p>Une stagiaire en développement web
qui aime le JavaScript tout particulièrement.</p>
    </div>
  </footer>
</template>

<script>
// Styles Pied de page
import "../styles/portfolio/PiedDePage.scss";
import "../assets/polices/Hudzaifah.otf";

export default {
  name: 'PiedDePage'
}
</script>