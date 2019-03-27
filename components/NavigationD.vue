<template lang="pug">
nav.navigation
  .primary
    .logo
      a.logo(v-scroll-to="'#primary-tout'")
        img(src="~assets/images/logo.png")
  .secondary
    a(v-scroll-to="'#primary-tout'") Home
    a(v-scroll-to="'#services'") Services
    a(v-scroll-to="'#about-us'") AboutUs
    //- nuxt-link(to="/Contact") Contact
</template>

<script>
import AOS from 'aos'
import 'aos/dist/aos.css'

import Vue from 'vue';
var VueScrollTo = require('vue-scrollto');
 
Vue.use(VueScrollTo)

export default {
  created () {
    AOS.init ({
      duration: 600
    })
  } 
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'

.navigation
  @include flex
  a.logo
    @include flex
    text-decoration: none
    color: $white
    img
      width: 10rem
      @media (max-width: $br-desktop-small)
        width: 10rem
        margin-left: $s*1.8
  .secondary
    position: relative
    a
      margin: 0 $s
      color: $tt-secondary-color

  .secondary
    @media (max-width: $br-tab-portrait)
      display: none
</style>
