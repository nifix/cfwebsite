<template>

<section id="aboutme" class="section about">
  <div class="container" v-scroll-reveal.reset>
    <div class="content">
      <h4 class="cat-header has-text-centered is-uppercase has-text-weight-semibold has-text-grey-dark">A PROPOS DE MOI</h4>
      <div class="columns">
        <div class="column is-5 is-offset-1">
          <h5 class="has-text-centered is-5">Qui suis-je ?</h5>
          <div class="aboutme-table">
            <div class="aboutme-item" style="padding-bottom: 2rem; height: 12rem;">
              <span class="is-hidden"></span>
              <p>Comptable de formation mais développeur dans l'ame depuis mes 15 ans, j'ai toujours considéré la programmation & l'informatique comme ma plus grande passion tout au long
              de ma vie.</p>
              <p>Je suis quelqu'un de travailleur et je ne compte pas mes heures afin que mes clients soient les plus satisfaits possible.</p>
            </div>
            <div class="aboutme-item">
              <span>Nom Prénom</span>
              <span>Fracassi Cédric</span>
            </div>
            <div class="aboutme-item">
              <span>Date de naissance</span>
              <span>15 Juillet 1988</span>
            </div>
            <div class="aboutme-item">
              <span>Professions</span>
              <span class="is-block">Développeur Web / VBA Freelance (10+ années)</span>
              <span>Comptable (5+ années)</span>
            </div>
            <div class="aboutme-item">
              <span>Domiciliation</span>
              <span>Marignane (13)</span>
            </div>
            <div class="aboutme-item">
              <span>Email</span>
              <span>cedric.fracassi@gmail.com</span>
            </div>
            <div class="aboutme-item">
              <span>Outils de développement</span>
              <span class="is-block">Visual Studio Code</span>
              <span class="is-block">Macbook</span>
              <span class="is-block">Github</span>
              <span class="is-block">Slack</span>
              <span class="is-block">.. Google</span>
            </div>
          </div>
        </div>
        <div class="column is-5">
          <h5 class="has-text-centered is-5 has-text-weight-semibold">Compétences</h5>

          <div class="aboutme-item-comp" style="padding-bottom: 2rem; height: 12rem;">
            <p>Originellement développeur PHP, la curiosité m'a poussé à m'orienter vers toute sorte de technologies.</p>
            <p>Le JavaScript est très présent et je suis actuellement en apprentissage de Flutter pour le développement d'applications pour mobile.</p>
          </div>

          <div class="aboutme-item-comp">
            <span>PHP 7 (88%)</span>
            <b-progress :value="88" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>VBA - Excel - Macros (85%)</span>
            <b-progress :value="85" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>HTML 5 - CSS 3 - SCSS - SASS (85%)</span>
            <b-progress :value="85" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>JavaScript - Webpack - Babel (80%)</span>
            <b-progress :value="80" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>PHP - Laravel (70%)</span>
            <b-progress :value="70" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>Python (70%)</span>
            <b-progress :value="70" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>Vue.js (70%)</span>
            <b-progress :value="70" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>Nuxtjs (70%)</span>
            <b-progress :value="70" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp" style="padding-top: 2rem; padding-bottom: 2rem;">
            <span>En cours d'apprentissage ...</span>
          </div>

          <div class="aboutme-item-comp">
            <span>Développement mobile - Flutter (35%)</span>
            <b-progress :value="35" size="is-small">
            </b-progress>
          </div>

          <div class="aboutme-item-comp">
            <span>ASP.Net Core 3 (35%)</span>
            <b-progress :value="20" size="is-small">
            </b-progress>
          </div>

        </div>
      </div>
    </div>
  </div>
</section>
</template>

<script>
export default {
}
</script>

<style>
.about {
   color: #1F1F1F;
}

.aboutme-table {
  flex-direction: row;
}

.aboutme-item {
  padding-bottom: 3px;
  padding-top: 3px;
  border-bottom: 1px solid rgba(0, 0, 0, .05);
  font-size: 0.95em;
}
.aboutme-item :first-child {
  display: block;
  width: 40rem;
  font-weight: 600;
}

.aboutme-item-comp {
  width: 100%;
  font-size: 0.95em;
  padding-bottom: 1rem;
}

</style>
