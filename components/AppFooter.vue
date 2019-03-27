<template lang="pug">
section.app-footer
  .container
    .contact
      .c-details
        p Bangalore,India
        span hello@targetthoughts.com | 98765 43219
    .s-links
      a
        img(src="~assets/images/facebook.png")
      a
        img(src="~assets/images/twitter.png")
      a
        img(src="~assets/images/linkedin.png")

</template>

<script>
export default {
  data () {
    return {

    }

  }

}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
section.app-footer
  background: $tt-secondary-color
  .container
    position: relative
    display: block
    text-align: center
    @media(min-width: $br-tab-portrait)
      @include flex
      padding: 0 !important
    .contact
      text-align: center
      .c-details
        @include flex
        justify-content: center
        @media(max-width: $br-tab-portrait)
          display: block
          font-size: 1rem
          margin: 0 auto
        p
          margin: 0 auto
          color: $white
          font-size: 1rem
          @media(max-width: $br-tab-portrait)
            margin-top: $s
            font-size: 0.8rem
        span
          color: $white
          margin-left: $s*20
          @media(max-width: $br-tab-portrait)
            margin: 0 auto
            margin-top: $s
            font-size: 0.7rem
    .s-links
      margin-top: $s
      a
        img
          margin-right: $s
          height: 1.25rem
          margin-bottom: $s
</style>


