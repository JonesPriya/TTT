<template lang="pug">
section#customers
  .primary
    .details
      h2 Customer
      .logo
        a.agi(href="https://americangarageinc.com/companies.html",target="_blank")
          img(src="~assets/images/c-logo.jpeg")
        span American Garage Inc


  
</template>

<script>

export default {
  
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
section#customers
  .primary
    padding-top: $s !important
    padding-bottom: $s*2 !important
    width: 50%
    margin: 0 auto
    @media (max-width: $br-tab-portrait)
      margin: 0 auto
      width: 100%
      display: inline-flex
    
    .logo
      img
        width: 60px
        height: 61.86px
        margin: 0 25px 0 0
      span
        font-size: 30px
        color: #00519F
        @media (max-width: $br-tab-portrait)
          font-size: 25px

    .details
      text-align: center
      @media (max-width: $br-tab-portrait)
        width: 100%
        margin-left: $s*4
        margin-right: $s*4
        h4
          @media (max-width: $br-tab-portrait)
            font-size: 1.2rem

</style>

