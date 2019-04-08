<template lang="pug">
.navigation(:class="{open: open}")
  ul.primary
    li
      a(v-scroll-to="'#primary-tout'", @click="clicked") Home
    li
      a(v-scroll-to="'#services'", @click="clicked") Services
    li
      a(v-scroll-to="'#customers'", @click="clicked") Customer
    li
      a(v-scroll-to="'#about-us'", @click="clicked") About Us
    //- li
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
    clicked () {
      this.$emit('clicked')
    }
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
    background: $tt-primary-color
    color: $white !important
    ul
      display: block

.primary
  @include reset
  margin-top: $s*6
  text-align: center

li
  margin: $s*3 !important
</style>