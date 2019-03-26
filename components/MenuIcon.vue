<template lang="pug">
.menu-icon(:class="{open: open}")
  span(v-for="(s, i) in 3", :key="i", :style="stylify(i)")
</template>

<script>
export default {
  props: {
    open: Boolean
  },
  methods: {
    stylify (i) {
      return {
        top: (i * 50) + '%'
      }
    }
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'

$icon-width: 2rem
$icon-height: 1rem

.menu-icon
  width: $icon-width
  height: $icon-height
  transform: rotate(0deg)
  transition: .5s ease-in-out
  @media (min-width: $br-tab-portrait)
    display: none
  &.open
    display: block
    transition: all 0.3s
  span
    display: block
    position: absolute
    height: 2px
    width: 100%
    background: $tt-secondary-color
    border-radius: 0.1rem
    opacity: 1
    left: 0
    transform: rotate(0deg)
    transition: .25s ease-in-out
    margin: 0

.menu-icon
  &.open
    span
      &:nth-child(2)
        width: 0
      &:nth-child(1)
        top: 50% !important
        transform: rotate(45deg)
      &:nth-child(3)
        top: 50% !important
        transform: rotate(-45deg)
</style>
