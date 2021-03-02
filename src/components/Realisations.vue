<template>
  <section class="Realisation">
    <h1>Mes réalisations</h1>
    <ul>
      <li>toutes</li>
      <li>web</li>
      <li>design</li>
      <li>autres</li>
    </ul>
    <!-- <img src="../assets/images/Denis_Marie-Lou_photoFinissante-blanche.jpg" alt=""> -->
    <ListeProjets/>
  </section>
</template>

<script>
import "../styles/portfolio/Realisations.scss";
import ListeProjets from './ListeProjets'
export default {
  name: 'Realisation',
  components: {
    'ListeProjets' : ListeProjets
  }
}
</script>