<template lang="pug">
.navigation(:class="{open: open}")
  ul.primary
    li
      nuxt-link(to="/Services") Services
    li
      nuxt-link(to="/AboutUs") AboutUs
    li
      nuxt-link(to="/Contact") Contact
</template>

<script>
import MenuIcon from './MenuIcon'

export default {
  props: {
    open: Boolean
  },
  data () {
    return {

    }
  },
  methods: {

  },
  components: {
    MenuIcon
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'

.navigation
  position: relative
  left: 100%
  overflow: hidden !important
  ul
    display: none
  &.open
    display: block
    @include fixed
    left: 0
    height: 100vh
    opacity: 1
    transition: all 0.3s
    background: $hm-neutral-dark
    color: $white !important
    ul
      display: block

.primary
  @include reset
  margin-top: 12rem
  text-align: center

li
  margin: $s*3 !important
</style>