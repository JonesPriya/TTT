<template lang="pug">
.page
  app-header
  primary-tout
  services
  about-us
  app-footer

</template>

<script>
import AppHeader from '~/components/AppHeader'
import PrimaryTout from '~/components/PrimaryTout'
import AboutUs from '~/components/AboutUs'
import Services from '~/components/Services'
import AppFooter from '~/components/AppFooter'


export default {
  components: {
    AppHeader,
    PrimaryTout,
    AboutUs,
    Services,
    AppFooter
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
</style>



