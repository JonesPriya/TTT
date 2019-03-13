<template lang="pug">
section.about-us
  .container
    .details
      h1 Enterprise Service Management
      p Target Thought Technologies offers ServiceNow as a Platform Experience which can transform your business elevating it to new heights of efficiency by streamlining workflows and facilitating a service-oriented approach across your enterprise.
      p We value quality over quantity so whether you're implementing ServiceNow for Enterprise Service, IT Operations Management or developing an app using the ServiceNow Platform, we take pride in being your most efficient, experienced and value-based option around.
  
</template>

<script>
export default {
  
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'

section.about
  background: $light-white

//section
.container
  padding-top: $s !important
  padding-bottom: $s*2 !important

  @media (max-width: 900px)
    display: inline-flex


  .details
    margin: $s
  @media (max-width: $br-desktop-small-1)
    width: 100%
    margin: $s*6 auto
  h2
    @media (max-width: $br-desktop-small)
      font-size: 1.5rem
      width: 100%

  p
    color: $hm-neutral-dark

</style>


