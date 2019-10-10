<template>

<header class="section intro">
  <div class="intro-text">
    <h5 class="subtitle is-5 has-text-grey-dark">Hello, world !</h5>
    <h1 class="title is-1 has-text-centered has-text-light" style="letter-spacing: 5px">{{ name }}</h1>
    <h5 class="subtitle is-5 job has-text-white">{{ job }}</h5>
    <b-button v-scroll-to="'#aboutme'" type="is-danger" outlined>En savoir plus</b-button>
    <div class="socialmedias">
      <a href="https://www.linkedin.com/in/cedric-fracassi" target="_blank" alt="Linkedin Cédric Fracassi">
        <font-awesome-icon swap-opacity :icon="['fab', 'linkedin']" />
      </a>
      <a class="social-mid" href="https://github.com/nifix" target="_blank" alt="Github Cédric Fracassi">
        <font-awesome-icon swap-opacity :icon="['fab', 'github']" />
      </a>
      <a href="mailto:cedric.fracassi@gmail.com" target="_blank" alt="Github Cédric Fracassi">
        <font-awesome-icon :icon="['fas', 'envelope']" />
      </a>
    </div>
  </div>
</header>

</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { fab } from '@fortawesome/free-brands-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'


library.add(fab)

export default {
  props: {
    name: {
      type: String,
      required: true
    },
    job: {
      type: String,
      required: true
    }
  }
}
</script>

<style>

.intro {
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.6) 0%, rgba(0, 0, 0, 1) 100%), url("~@/assets/bg-universe-opti.jpg") no-repeat center bottom;
  background-size: cover;
  width: 100%;
  height: 100%;
  min-height: 100vh;
  margin: 0;
  position: relative;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.intro .intro-text {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.intro * {
  color: #F5F5F5;
}

.intro h5 {
  padding-bottom: 0.4rem;
  text-transform: uppercase;
}

.intro h1 {
  padding: 1.4rem 0rem 1.4rem 0rem;
}

.socialmedias {
  padding-top: 2.4rem;
  font-size: 2.5rem;
  display:flex;
}

.socialmedias .social-mid {
  padding-left: 3rem;
  padding-right: 3rem;
}
</style>
