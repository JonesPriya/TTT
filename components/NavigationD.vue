<template lang="pug">
nav.navigation
  .primary
    nuxt-link.logo(to="/")
      img(src="~assets/images/logo.png")
  .secondary
    a(v-scroll-to="'#services'") Services
    a AboutUs
    nuxt-link(to="/Contact") Contact
</template>

<script>
import AOS from 'aos'
import 'aos/dist/aos.css'

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
  img
    width: 10rem
.secondary
  position: relative
  a
    margin: 0 $s

.secondary
  @media (max-width: $br-tab-portrait)
    display: none
</style>
