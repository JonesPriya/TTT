<template lang="pug">
.page
  app-header
  c-hero
  c-details
  
</template>

<script>
import AppHeader from '~/components/AppHeader'
import CHero from '~/components/contact/CHero'
import CDetails from '~/components/contact/CDetails'
export default {
  components: {
    AppHeader,
    CHero,
    CDetails
  }
  
}
</script>

<style lang="sass" scoped>

</style>



