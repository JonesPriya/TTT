<template lang="pug">
.app-header
  .container
    a.hamburger(@click="toggle()")
      menu-icon.icon(:open="show")
    navigation-d.desktop
    navigation-m.mobile(:open="show")
</template>

<script>
import MenuIcon from './MenuIcon'
import NavigationD from '~/components/NavigationD'
import NavigationM from '~/components/NavigationM'

export default {
  data () {
    return {
      show: false
    }
  },
  methods: {
    toggle () {
      this.show = !this.show
    }
  },
  components: {
    NavigationD,
    NavigationM,
    MenuIcon,
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'


.app-header
  @include fixed-n
  background: $hm-neutral-dark
  z-index: 4
  height: 5.5rem
  color: $white
  overflow: visible
  @media (max-width: $br-tab-portrait)
    transition: .5s ease
    height: 5rem
    &.open
      height: 100%

  .container
    padding: 0 0 !important

a.hamburger
  display: block
  @include fixed-ne($s*2)
  z-index: 1000000

.icon.open
  display: block

// .desktop
//   @media (max-width: $br-tab-portrait)
//     display: none
.mobile
  @media (min-width: $br-tab-portrait)
    display: none

.container
  position: relative
  max-width: $page-width-wide
  overflow-x: hidden
  margin: 0 auto
  padding: $s*1 0
  @media (max-width: $br-desktop-wide)
    max-width: $page-width
  @media (max-width: $br-tab-portrait)
    padding: 0 $s*2
  @media (max-width: $br-desktop-small)
    padding: 0 $s*2
</style>