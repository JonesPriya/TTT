<template lang="pug">
section.c-hero
  .mask
  .container
    .content
      h1 Contact Us
</template>

<script>
export default {
  
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
section.c-hero
  position: relative
  overflow: visible !important
  background-image: url('~assets/images/bg.jpg')
  background-size: cover
  background-position: center center
  background-repeat: no-repeat
  height: 100vh
  @media (max-width: $br-tab-portrait)
    height: 75vh
  
  .mask
    background-color: rgba($tt-neutral-dark, 0.7)
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
  color: #fff
  margin-top: $s*14
  width: 100%
  text-align: center
  @media(max-width: $br-tab-portrait)
    width: 100%
    height: 32rem
  h1
    margin-top: $s*5
    @media(max-width: $br-tab-portrait)
      font-size: 1.5rem !important
      margin-top: $s*5
      margin-bottom: $s

</style>


