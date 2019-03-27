<template lang="pug">
section#services
  .container
    .heading
      h1 Our services
      p Our team of certified experts can help you with
    .details
      .content(v-for="s, i in service", :key="i")
        .icon()
          img(:src="getImageurl(s.icon)")
        h4 {{ s.title }}
        p {{ s.description }}
      //- view-services(@toggle="toggle()")
</template>

<script>
import service from 'static/data/service.js'
// import ViewServices from './ViewServices'
export default {
  data () {
    return {
      service: service
    }
  },
   methods: {
    getImageurl (icon) {
      return require('../assets/images/' + icon)
    },
//     toggle () {
//       this.expanded = !this.expanded
//     }
//   },
//   components: {
//     ViewServices
  }
}
</script>

<style lang="sass" scoped>
@import 'assets/styles/includes'
.container
  // min-height: 100vh
  &:last-child
    border-bottom: none
  .heading
    text-align: center
    width: 50%
    margin: 0 auto
    @media (max-width: $br-tab-portrait)
      width: 100%
      margin: $s*3 0
    h1
      padding-top: $s*2
      @media (max-width: $br-tab-portrait)
        margin-bottom: $s
        font-size: 1.5rem
    
    ::before
      @include absolute-n
      top: $s*10
      content: " "
      height: 0.1rem
      width: 4rem
      border: 1px solid $tt-primary-color
      border-radius: 5rem
      opacity: 0.3
      @media (max-width: $br-tab-portrait)
        top: $s*8

    p
      margin-bottom: $s*3
      line-height: 1.5rem

.details
  @include flex(center, center)
  flex-wrap: wrap
  align-items: flex-start
  margin-bottom: $s
  @media (max-width: $br-tab-portrait)
    display: block
  .content
    max-width: 33.33%
    padding: $s*1.5
    text-align: center
    position: relative
    h4
      margin-bottom: 1.6rem
      margin-top: 2.5rem
      font-weight: 500
      font-size: 1.1rem

    @media (max-width: $br-tab-portrait)
      max-width: 100%
      padding: 1rem
      h4
        font-size: 1rem
      p
        width: 100%
    .icon
      @include absolute
      width: 2.5rem
      img
        width: 2rem
        @media (max-width: $br-tab-portrait)
          margin-bottom: 3rem

    p
      margin-top: $s*2
      line-height: 1.5rem

</style>