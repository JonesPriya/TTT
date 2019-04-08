<template lang="pug">
section#primary-tout
  //- .mask
  .container
    .content
      h1(data-aos="fade-up") ServiceNow
      h4(data-aos="fade-up") your preferred service management specialists
</template>

<script>


export default {
  data () {
    return {

    }
  },
  methods: {

  },
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
section#primary-tout
  position: relative
  overflow: visible !important
  background-image: url('~assets/images/ttt-hero-banner.jpg')
  background-size: cover
  background-position: center center
  background-repeat: no-repeat
  height: 100vh
  @media (max-width: $br-tab-portrait)
    height: 75vh
  
  // .mask
    background-color: rgba($tt-primary-color, 0.5)
    @include absolute

.container
  overflow: visible !important
  @media(max-width: $br-tab-portrait)
    position: relative
    @include flex
    overflow: visible !important
    height: 30rem
    justify-content: unset
    padding: 0 $s*2
.content
  color: $white
  margin-top: $s*14
  width: 100%
  @media(max-width: $br-tab-portrait)
    width: 100%
    height: 32rem
  h1
    margin-top: $s*5
    font-size: 3rem
    font-weight: 500
    @media(max-width: $br-tab-portrait)
      font-size: 1.5rem !important
      margin-top: $s*5
      margin-bottom: $s
  h4
    margin-bottom: $s*4
    color: $white
    font-weight: 500
    font-size: 1rem
    line-height: 0.55rem
    @media(max-width: $br-tab-portrait)
      line-height: 1.2rem


</style>
