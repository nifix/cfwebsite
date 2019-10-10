<template>

<footer id="footer" class="section footer has-background-white-bis has-text-white-ter has-text-centered" >
  <div class="container" v-scroll-reveal.reset>
    <div class="content is-centered">
      <div style="padding-bottom: 2rem;" class="has-text-info">Made with love by Cédric Fracassi with Nuxtjs, Bulma. Hosted on Netlify.</div>
      <div class="socialmedias-footer">
        <a href="https://www.linkedin.com/in/cedric-fracassi" target="_blank" alt="Linkedin Cédric Fracassi">
          <font-awesome-icon swap-opacity :icon="['fab', 'linkedin']" />
        </a>
        <a class="social-mid" href="https://github.com/nifix" target="_blank" alt="Github Cédric Fracassi">
          <font-awesome-icon swap-opacity :icon="['fab', 'github']" />
        </a>
        <a href="mailto:cedric.fracassi@gmail.com" target="_blank" alt="Github Cédric Fracassi">
          <font-awesome-icon swap-opacity :icon="['fas', 'envelope']" />
        </a>
      </div>
    </div>
  </div>
</footer>


</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { fab } from '@fortawesome/free-brands-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

library.add(fab)

export default {

}
</script>

<style>
.socialmedias-footer {
  font-size: 2.5rem;
  display:flex;
  justify-content: center;
  align-items: middle;
}

.socialmedias-footer .social-mid {
  padding-left: 3rem;
  padding-right: 3rem;
}
</style>
