<template lang="pug">
section#services
  .container
      .heading
        h1 Our services
        p Our team of certified experts can help you with
      .details
        .content(v-for="s, i in service", :key="i")
          .icon
            img(:src="getImageurl(s.icon)")
          h4 {{ s.title }}
          p {{ s.description }}
</template>

<script>
import service from 'static/data/service.js'
export default {
  data () {
    return {
      service: service
    }
  },
   methods: {
    getImageurl (icon) {
      return require('../assets/images/' + icon)
    }
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
      text-align: left
      margin: $s*3 0
    h1
      padding-top: $s*2
      @media (max-width: $br-tab-portrait)
        margin-bottom: $s
        font-size: 1.5rem

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
    @media (max-width: $br-tab-portrait)
      max-width: 100%
      padding: 0
      h4
        font-size: 1rem
      p
        width: 100%
      .icon
        padding: $s/4

    p
      margin-top: $s*2
      line-height: 1.5rem
      font-size: 0.8rem

</style>