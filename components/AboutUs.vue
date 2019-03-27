<template lang="pug">
section#about-us
  .about
    .details
      h4 Enterprise Service Management
      p Target Thought Technologies offers ServiceNow as a Platform Experience which can transform your business by streamlining workflows and facilitating service-oriented approach across your enterprise.We value quality over quantity. 
</template>

<script>
export default {
  
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'

section#about-us
  background: $light-white

//section
.about
  padding-top: $s !important
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
      h4
        @media (max-width: $br-tab-portrait)
          font-size: 1.2rem

</style>


