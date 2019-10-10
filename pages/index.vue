<template>
  <div>
    <Landing :name="name" :job="job" />
    <About />
    <Resume />
    <Portfolio />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Landing from '~/components/Landing'
import About from '~/components/About'
import Resume from '~/components/Resume'
import Portfolio from '~/components/Portfolio'
import Contact from '~/components/Contact'
import Footer from '~/components/Footer'

export default {
  data () {
    return {
      name: 'Cédric Fracassi',
      job: 'Développeur Web Full Stack'
    }
  },

  head () {
    return {
      title: 'Cédric Fracassi - Développeur Web Full Stack Freelance',
      description: 'Développeur Web FullStack/VBA Freelance, si vous avez un problème en informatique, je trouverai une solution.'
    }
  },

  components: {
    Landing,
    About,
    Resume,
    Portfolio,
    Contact,
    Footer
  }
}
</script>

<style type="scss">
* {
  font-family: 'Roboto', sans-serif;
}

body, html {
    -webkit-font-smoothing: antialiased;
    min-width: 300px;
    height: auto;
    overflow-x: hidden;
    text-rendering: optimizeLegibility;
    text-size-adjust: 100%;
}
.cat-header {
  letter-spacing: 5px;
  color: #cc005f;
  padding-bottom: 1.4rem;
}
</style>

