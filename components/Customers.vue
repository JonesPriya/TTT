<template lang="pug">
section#customers
  .primary
    .details
      h4 Customer
      .logo
        a.agi(href="https://americangarageinc.com/companies.html",target="_blank")
          img(src="~assets/images/c-logo.png")


  
</template>

<script>

export default {
  
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
section#customers
  @media (max-width: $br-tab-portrait)
    width: 20rem
  .primary
    // padding-top: $s !important
    padding-bottom: $s*2 !important
    width: 50%
    margin: 0 auto
    @media (max-width: $br-tab-portrait)
      margin: 0 auto
      width: 100%
      display: inline-flex
    .details
      text-align: center
      @media (max-width: $br-tab-portrait)
        width: 100%
        margin-left: $s*4
        margin-right: $s*4
        margin-top: $s*4
        
      h4
        font-size: 1.3rem
        line-height: 1.6rem
        margin: 1.2rem 0 1.6rem
        @media (max-width: $br-tab-portrait)
          font-size: 1.2rem
      .logo
        img
          width: 18rem
</style>

