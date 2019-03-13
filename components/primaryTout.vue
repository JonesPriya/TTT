<template lang="pug">
section.primary-tout
  .container
    .content
      h1(data-aos="fade-up") ServiceNow
      p(data-aos="fade-up") your preferred service management specialists
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
section.primary-tout
  // background-color: $hm-pink
  overflow: visible !important
  background-image: url('~assets/images/bg.png')
  background-size: cover
  background-position: center center
  background-repeat: no-repeat
  @media (max-width: $br-tab-portrait)
    height: 75vh

.container
  overflow: visible !important
  @media(min-width: $br-tab-portrait)
    position: relative
    @include flex
    overflow: visible !important
    height: 39rem
    justify-content: unset
.content
  color: #000
  margin-top: $s
  width: 100%
  text-align: center
  @media(max-width: $br-tab-portrait)
    width: 100%
    margin-top: $s*2
  h1
    margin-top: $s*5
    @media(max-width: $br-tab-portrait)
      font-size: 1.5rem !important
      margin-top: $s*5
      margin-bottom: $s
  p
    margin-bottom: $s*4
    color: #000
    line-height: 1.55rem
    text-transform: uppercase

</style>
