<template lang="pug">
.page
  app-header
  primary-tout
  services
  customers
  about-us
  app-footer

</template>

<script>
import AppHeader from '~/components/AppHeader'
import PrimaryTout from '~/components/PrimaryTout'
import AboutUs from '~/components/AboutUs'
import Services from '~/components/Services'
import Customers from '~/components/Customers'
import AppFooter from '~/components/AppFooter'


export default {
  components: {
    AppHeader,
    PrimaryTout,
    AboutUs,
    Services,
    Customers,
    AppFooter
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
</style>



