<template>

<section id="portfolio" class="section portfolio">
  <div class="container" v-scroll-reveal.reset>
    <div class="content is-centered">
      <h4 class="cat-header has-text-centered is-full is-uppercase has-text-weight-semibold has-text-grey-dark">Portfolio</h4>

      <div class="columns is-centered is-multiline">

        <div  class="column is-12-mobile is-half-tablet is-one-quarter-desktop">
          <figure class="image is-3by2">
            <img src="~@/assets/thumbnail_portfolio-opti.jpg" alt="Image du site personnel de Cédric Fracassi">
            <div class="portfolio-item-overlay" style="vertical-align:middle">
              <p class="label">Site personnel, développé avec Vue.js, Nuxtjs & Bulma</p>
            </div>
          </figure>
        </div>

        <div class="column is-12-mobile is-half-tablet is-one-quarter-desktop">
          <figure class="image is-3by2">
            <img src="~@/assets/thumbnail_caisseace.jpg" alt="Application caisse Espace ACE">
            <div class="portfolio-item-overlay" style="vertical-align:middle">
              <p class="label">(C#) Application de parse de la caisse</p>
              <span class="is-block"><b-button type="is-danger" @click="launchUri('https://github.com/nifix/ace-caisse')" outlined>Voir sur Github</b-button></span>
            </div>
          </figure>
        </div>

        <div class="column is-12-mobile is-half-tablet is-one-quarter-desktop">
          <figure class="image is-3by2">
            <img src="~@/assets/thumbnail_alextaxi-sumup.jpg" alt="Alex-Taxi Export Python">
            <div class="portfolio-item-overlay" style="vertical-align:middle">
              <p class="label is-block">(Python) Export automatique des opérations de CB</p>
              <span class="is-block"><b-button type="is-danger" @click="launchUri('https://github.com/nifix/Divers/blob/master/Python%20-%20Alex%20Taxi%20-%20Export%20transactions/ace-alextaxi-export-cb.py')" outlined>Voir sur Github</b-button></span>
            </div>
          </figure>
        </div>

        <div class="column is-12-mobile is-half-tablet is-one-quarter-desktop">
          <figure class="image is-3by2">
            <img src="~@/assets/thumbnail_tool-cfe.jpg" alt="Outil de traitement de la CFE 2018 (Espace ACE)">
            <div class="portfolio-item-overlay" style="vertical-align:middle">
              <p class="label is-block">(VBA) Outil de traitement de la CFE 2018</p>
              <span class="is-block"><b-button type="is-danger" @click="launchUri('https://github.com/nifix/Divers/blob/master/VBA%20-%20CFE%202018.xlsm')" outlined>Voir sur Github</b-button></span>
            </div>
          </figure>
        </div>


        <div class="column is-12-mobile is-half-tablet is-one-quarter-desktop">
          <figure class="image is-3by2">
            <img src="~@/assets/thumbnail_tool-qonto.jpg" alt="Outil de traitement des relevés Qonto (Espace ACE)">
            <div class="portfolio-item-overlay" style="vertical-align:middle">
              <p class="label is-block">(VBA) Outil de traitement des relevés bancaires Qonto</p>
              <span class="is-block"><b-button type="is-danger" @click="launchUri('https://github.com/nifix/Divers/blob/master/VBA%20-%20FOLIMAGE%20-%20Relev%C3%A9%20Qonto.xlsm')" outlined>Voir sur Github</b-button></span>
            </div>
          </figure>
        </div>

        <div class="column is-12-mobile is-half-tablet is-one-quarter-desktop">
          <figure class="image is-3by2">
            <img src="~@/assets/thumbnail_tool-cheaterheroes.jpg" alt="Script d'édition de sauvegarde du jeu ClickerHeroes">
            <div class="portfolio-item-overlay" style="vertical-align:middle">
              <p class="label is-block">(PHP/Python) Script d'édition de sauvegarde du jeu ClickerHeroes</p>
              <span class="is-block"><b-button type="is-danger" @click="launchUri('https://github.com/nifix/CheaterHeroes')" outlined>Voir sur Github</b-button></span>
            </div>
          </figure>
        </div>

        <div class="column is-12-mobile is-half-tablet is-one-quarter-desktop">
          <figure class="image is-3by2">
            <img src="~@/assets/thumbnail_github.jpg" alt="Lien vers le Github de Cédric Fracassi">
            <div class="portfolio-item-overlay" style="vertical-align:middle">
              <p class="label is-block">Découvrez mes projets sur Github !</p>
              <span class="is-block"><b-button type="is-danger" @click="launchUri('https://github.com/nifix')" outlined>Découvrir</b-button></span>
            </div>
          </figure>
        </div>

      </div>

    </div>
  </div>
</section>

</template>

<script>
export default {
  methods:{
    launchUri: (url) => {
      window.open(url);
    },
  }
}
</script>

<style>

.portfolio {
  color: #1F1F1F;
  font-size: 0.85em;
}

.portfolio figure .portfolio-item-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  background-color: #293347;
  -webkit-transition: .5s ease;
  transition: .5s ease;
  opacity: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.portfolio figure .portfolio-item-overlay:hover {
  opacity: 1;
}

.portfolio figure .portfolio-item-overlay .label {
  color: #FFFFFF;
  margin: 1rem;
}

.portfolio figure {
  overflow: hidden;
  border-radius: 12px;
  border: 1px solid #d3d3d3;
}

</style>
